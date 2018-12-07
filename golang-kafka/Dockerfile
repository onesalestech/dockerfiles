FROM quay.io/onesalestech/golang:latest

LABEL maintainer "ONE <tech@onet.io>"

RUN git clone -b 0.11.x https://github.com/edenhill/librdkafka.git
RUN cd librdkafka && ./configure --prefix=/usr && make && make install
