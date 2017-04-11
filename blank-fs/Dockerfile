FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget $(wget https://api.github.com/repos/getblank/blank-fs/releases/latest -O- | grep 'browser_' | cut -d\" -f4 | grep linux) -O /bin/blank-fs \
&& chmod +x /bin/blank-fs \
&& mkdir /app

WORKDIR /app
EXPOSE 8082
CMD blank-fs -s ws://blank-sr:1234