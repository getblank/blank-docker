FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget http://releases.getblank.net/blank-cron/linux/blank-cron -O /bin/blank-cron \
&& chmod +x /bin/blank-cron

CMD blank-cron -s ws://blank-sr:1234