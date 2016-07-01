FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget http://releases.getblank.net/blank-queue/linux/blank-queue -O /bin/blank-queue \
&& chmod +x /bin/blank-queue && mkdir /app

WORKDIR /app

CMD blank-queue -s ws://blank-sr:1234