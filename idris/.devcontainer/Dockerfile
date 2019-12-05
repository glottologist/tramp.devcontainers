FROM glottologist/development-centos:19.12.3
ENV PATH="${HOME}/.local/bin:$HOME/.cabal/bin:${PATH}"
ADD README.md .
ADD hello.idr .


RUN  yum -y install curl-devel expat-devel gettext-devel openssl-devel zlib-devel perl-ExtUtils-MakeMaker gcc-c++ make gmp-devel

# Install newer version of git than the package manager provides
RUN mkdir -p /usr/local/source \
    && cd /usr/local/source \
    && wget https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.9.5.tar.gz \
    && tar -xvf git-2.9.5.tar.gz \
    && cd git-2.9.5 \
    && ./configure \
    && make \
    && make install


RUN yum -y  install idris

RUN idris hello.idr -o hello
