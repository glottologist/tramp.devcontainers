FROM glottologist/development-ubuntu:19.12.3
ADD README.md .
ENV PATH="/usr/local/go/bin:$PATH"
RUN wget https://dl.google.com/go/go1.12.9.linux-amd64.tar.gz && \
    tar -C /usr/local -xzf go1.12.9.linux-amd64.tar.gz && \
    echo $(go version)