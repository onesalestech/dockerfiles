FROM quay.io/onesalestech/golang:latest

LABEL maintainer "ONE <tech@onet.io>"

RUN git clone https://github.com/edenhill/librdkafka.git
RUN cd librdkafka && git checkout tags/v0.11.6 && ./configure --prefix=/usr && make && make install
