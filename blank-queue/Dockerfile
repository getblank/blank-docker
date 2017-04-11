FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget $(wget https://api.github.com/repos/getblank/blank-queue/releases/latest -O- | grep 'browser_' | cut -d\" -f4 | grep linux) -O /bin/blank-queue \
&& chmod +x /bin/blank-queue && mkdir /app

WORKDIR /app
CMD blank-queue -s ws://blank-sr:1234