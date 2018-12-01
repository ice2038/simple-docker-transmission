# ice2038/simple-docker-transmission [![Build Status](https://travis-ci.org/ice2038/simple-docker-transmission.svg?branch=master)](https://travis-ci.org/ice2038/simple-docker-transmission)

Dockerized Lightweight BitTorrent client (daemon and webinterface). [Transmission](http://www.transmissionbt.com/about/)

## Usage

```
$ cat simple-docker-transmission/Dockerfile
$ docker build -t simple-docker-transmission simple-docker-transmission
$ docker run --rm -it -p 9091:9091 -p 55555:55555 \
    -v /tmp/downloads:/data/downloads ice2038/simple-docker-transmission

```

## Build it yourself

```
$ docker run -d --name transmission -p 9091:9091 -p 55555:55555 \
    -v /tmp/downloads:/data/downloads ice2038/simple-docker-transmission

```