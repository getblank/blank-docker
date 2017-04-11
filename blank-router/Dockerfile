FROM getblank/busybox
MAINTAINER Opryshko Alexandr <sclif13@gmail.com>

RUN wget $(wget https://api.github.com/repos/getblank/blank-router/releases/latest -O- | grep 'browser_' | cut -d\" -f4 | grep linux) -O /bin/blank-router \
&& chmod +x /bin/blank-router

EXPOSE 2345

CMD blank-router -s ws://blank-sr:1234