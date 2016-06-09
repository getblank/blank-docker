FROM golang:1.6
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN go get -u github.com/getblank/blank-sr && mkdir /app

EXPOSE 1234

WORKDIR /app

CMD blank-sr
