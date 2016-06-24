FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget http://releases.getblank.net/blank-router/linux/blank-router -O /bin/blank-router \
&& chmod +x /bin/blank-router

EXPOSE 2345

CMD blank-router -s ws://blank-sr:1234