# Docker Raspbian Image

[![Docker Build Status](https://img.shields.io/docker/cloud/build/xzaero/raspbian?color=green&style=flat-square)](https://hub.docker.com/r/xzaero/raspbian/)
[![Docker Build Status](https://img.shields.io/docker/pulls/xzaero/raspbian?style=flat-square)](https://hub.docker.com/r/xzaero/raspbian/)

This docker image runs QEMU system emulation for Raspbian Lite.
It will let you run Raspbian as if it was running on an actual Raspberry PI, including the CPU architecture.

## Usage

SSH is enabled on port `2222`. The username is `pi` and the password is `raspberry`.

To run the container:

`docker run -it -p 2222:2222 --privileged xzaero/raspbian`

To connect with SSH:

`ssh -p 2222 -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no pi@localhost`
