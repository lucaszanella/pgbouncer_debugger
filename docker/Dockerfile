FROM ubuntu:bionic

WORKDIR /home/project

RUN export DEBIAN_FRONTEND=noninteractive && apt-get update && apt-get install -y make build-essential\
    libevent-dev libssl-dev pkg-config autoconf libtool pandoc git python gdb

RUN git clone https://github.com/pgbouncer/pgbouncer.git\
    && cd pgbouncer\
    && git submodule init\
    && git submodule update\
    && ./autogen.sh \
    && ./configure ... \
    && make
    #&& make install