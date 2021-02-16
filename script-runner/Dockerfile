FROM alpine:3.13
LABEL maintainer="Mindship <asif@mindship.io>"
RUN apk update
RUN apk add curl ca-certificates
WORKDIR /script
COPY ./script.sh /script/
COPY ./curlrc /script/.curlrc
ENTRYPOINT ["sh","script.sh"]
