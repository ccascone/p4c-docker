# Docker-based distribution of p4c

Minimal Docker image with the open source P4 compiler (p4c) that includes the
following backends:

* `p4c-bm-ss`: BMv2 simple_switch backend;
* `p4c-graphs`: graphs generator.

This image was created to facilitate the compilation of P4 programs distributed
with the ONOS SDN controller, but you can use it without ONOS.

To obtain the image:

    docker pull ccasconeonf/p4c:<tag>

## Tags

The image comes in two tags:

* `ccasconeonf/p4c:latest` Updated daily and built from the master branch of
  the [p4lang/p4c][p4c] repository;
* `ccasconeonf/p4c:stable` Built using an arbitrary selected p4c commit that
  produces outputs known to work well with the ONOS development and testing
  environment.

## Status [![Build Status](https://travis-ci.org/ccascone/p4c-docker.svg?branch=master)](Travis)

Images are built daily using [Travis CI][Travis] and pushed to 
[Docker Hub][Docker Hub].

[![](https://images.microbadger.com/badges/version/ccasconeonf/p4c:latest.svg)](https://microbadger.com/images/ccasconeonf/p4c:latest)
[![](https://images.microbadger.com/badges/image/ccasconeonf/p4c:latest.svg)](https://microbadger.com/images/ccasconeonf/p4c:latest)

[![](https://images.microbadger.com/badges/version/ccasconeonf/p4c:stable.svg)](https://microbadger.com/images/ccasconeonf/p4c:stable)
[![](https://images.microbadger.com/badges/image/ccasconeonf/p4c:stable.svg)](https://microbadger.com/images/ccasconeonf/p4c:stable)

[Travis]: https://travis-ci.org/ccascone/p4c-docker
[Docker Hub]: https://hub.docker.com/r/ccasconeonf/p4c
[p4c]: https://github.com/p4lang/p4c