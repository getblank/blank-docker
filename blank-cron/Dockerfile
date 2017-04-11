FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget $(wget https://api.github.com/repos/getblank/blank-cron/releases/latest -O- | grep 'browser_' | cut -d\" -f4 | grep linux) -O /bin/blank-cron \
&& chmod +x /bin/blank-cron

CMD blank-cron -s ws://blank-sr:1234