FROM glottologist/development-ubuntu:19.12.3
ADD README.md .
ENV PATH="/v-master:${PATH}"
RUN apt-get install -y make && \
    wget https://github.com/vlang/v/archive/master.zip && \
    unzip master.zip && \
    cd v-master && \
    make

