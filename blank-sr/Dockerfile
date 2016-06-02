FROM golang:1.6
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN go get -d github.com/getblank/blank-sr && cd $GOPATH/src/github.com/getblank/blank-sr && go get -u -v && go install

WORKDIR /go/bin

EXPOSE 1234

CMD ["./blank-sr"]
