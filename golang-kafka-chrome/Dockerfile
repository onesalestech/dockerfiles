FROM quay.io/onet/golang-kafka:1.12.1

LABEL maintainer "Onet <tech@onet.io>"

RUN \
  apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* \
  && apt-get update -y \
  && apt-get install -y libnspr4 libnss3 libexpat1 libfontconfig1 libuuid1 \
  && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* 

RUN mkdir -p /headless-shell/
WORKDIR /headless-shell/
RUN wget https://dev-static-public-onet.s3.amazonaws.com/headless-shell/headless_shell
RUN chmod +x headless_shell
RUN mkdir -p swiftshader
WORKDIR /headless-shell/swiftshader
RUN wget https://dev-static-public-onet.s3.amazonaws.com/headless-shell/swiftshader/libEGL.so
RUN wget https://dev-static-public-onet.s3.amazonaws.com/headless-shell/swiftshader/libEGL.so.TOC
RUN wget https://dev-static-public-onet.s3.amazonaws.com/headless-shell/swiftshader/libGLESv2.so
RUN wget https://dev-static-public-onet.s3.amazonaws.com/headless-shell/swiftshader/libGLESv2.so.TOC
