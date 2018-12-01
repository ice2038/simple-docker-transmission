# ice2038/simple-docker-transmission [![Docker Automated build](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://hub.docker.com/r/ice2038/simple-docker-transmission/) [![Build Status](https://travis-ci.org/ice2038/simple-docker-transmission.svg?branch=master)](https://travis-ci.org/ice2038/simple-docker-transmission) [![](https://images.microbadger.com/badges/image/ice2038/simple-docker-transmission.svg)](https://microbadger.com/images/ice2038/simple-docker-transmission "Get your own image badge on microbadger.com") [![](https://images.microbadger.com/badges/version/ice2038/simple-docker-transmission.svg)](https://microbadger.com/images/ice2038/simple-docker-transmission "Get your own version badge on microbadger.com")

Dockerized Lightweight BitTorrent client (daemon and webinterface). [Transmission](http://www.transmissionbt.com/about/)

## Usage

```
$ docker run --rm -it -p 9091:9091 -p 55555:55555 \
    -v /tmp/downloads:/data/downloads ice2038/simple-docker-transmission
```

## Build it yourself

```
$ git clone git@github.com:ice2038/simple-docker-transmission.git
$ cd simple-docker-transmission.git
$ cat Dockerfile
$ docker build -t simple-docker-transmission .
$ docker run -d --name transmission -p 9091:9091 -p 55555:55555 \
    -v /tmp/downloads:/data/downloads simple-docker-transmission
```