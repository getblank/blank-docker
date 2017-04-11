FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget $(wget https://api.github.com/repos/getblank/blank-sr/releases/latest -O- | grep 'browser_' | cut -d\" -f4 | grep linux) -O /bin/blank-sr \
&& chmod +x /bin/blank-sr \
&& mkdir /app

EXPOSE 1234
WORKDIR /app
CMD blank-sr
