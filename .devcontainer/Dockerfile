FROM mcr.microsoft.com/devcontainers/base:noble

RUN apt-get update && \
    export DEBIAN_FRONTEND=noninteractive && \
    apt-get -y install \
        gcc-aarch64-linux-gnu \
        bc \
        flex \
        bison \
        cpio \
        file \
        uthash-dev

RUN cd /tmp && \
    git clone https://github.com/jduck/lk-reducer.git && \
    cd lk-reducer && \
    make && \
    cp lk-reducer /bin && \
    rm -rf /tmp/lk-reducer
