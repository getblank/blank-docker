FROM golang:1.6
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN go get -u github.com/getblank/blank-filestore && mkdir /app

WORKDIR /app

CMD blank-filestore -s ws://blank-sr:1234
