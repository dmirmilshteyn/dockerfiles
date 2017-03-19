FROM debian:wheezy

ENV PATH:$PATH
RUN apt-get update \
    && apt-get install -y -qq git autoconf libtool automake build-essential mono-devel gettext cmake \
    && PATH="/opt/mono/bin":$PATH \
    && git clone https://github.com/mono/mono.git \
    && cd mono \
    && ./autogen.sh --prefix="/opt/mono" \
    && make \
    && make install