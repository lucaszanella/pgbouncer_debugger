FROM ubuntu:bionic

WORKDIR /home/project

RUN export DEBIAN_FRONTEND=noninteractive && apt-get update && apt-get install -y make build-essential\
    libevent-dev libssl-dev pkg-config autoconf libtool pandoc git python gdb patch python-dev python3-dev\
    python3 postgresql postgresql-contrib


#RUN git clone https://github.com/pgbouncer/pgbouncer.git --branch "pgbouncer_1_12_0"\
#    && git clone https://github.com/awslabs/pgbouncer-rr-patch.git
#    && cd pgbouncer-rr-patch\
#    && ./install-pgbouncer-rr-patch.sh ../pgbouncer\
#    && cd ../pgbouncer\
#    && git submodule init\
#    && git submodule update\
#    && ./autogen.sh\
#    && ./configure ...\
#    && make\
#    && make install