# blank-docker
Docker containers for Blank

## Install docker-compose

```bash
curl -L https://github.com/docker/compose/releases/download/1.7.1/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```

## Running multi-containers

```bash
git clone https://github.com/getblank/blank-docker.git
cd blank-docker
docker-compose build
docker-compose up -d
```
