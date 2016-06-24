FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget http://releases.getblank.net/blank-sr/linux/blank-sr -O /bin/blank-sr \
&& chmod +x /bin/blank-sr \
&& mkdir /app

EXPOSE 1234
WORKDIR /app
CMD blank-sr
