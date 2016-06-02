FROM golang:1.6
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN go get -u github.com/jteeuwen/go-bindata/...

RUN go get -d github.com/getblank/blank-router \
&& cd $GOPATH/src/github.com/getblank/blank-router \
&& go generate \
&& go get -u -v \
&& go install

WORKDIR /go/bin

EXPOSE 2345

CMD ./blank-router -s ws://blank-sr:1234