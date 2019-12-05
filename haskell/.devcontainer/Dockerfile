FROM glottologist/development-ubuntu:19.12.3
RUN curl -sSL https://get.haskellstack.org/ -o install_stack.sh \
    && sh install_stack.sh \
    && stack upgrade --binary-only \
    && stack install hlint \
    && stack setup 





