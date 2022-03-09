# Vagrant Ubuntu

[![docker pull apax/bionic-vagrant](https://img.shields.io/badge/dockerhub-image-blue.svg?logo=Docker)](https://hub.docker.com/repository/docker/apax/bionic-vagrant)

This is the source Dockerfile for the [apax/bionic-vagrant](https://hub.docker.com/repository/docker/apax/bionic-vagrant) docker image.

## Building / Tagging
To build the Ubuntu 18.04 image for both arm and x86:

```bash
docker buildx build --push --platform linux/arm64,linux/amd64 -t apax/vagrant-ubuntu:18.04 -f Dockerfile.bionic .
```


To build the Ubuntu 20.04 image for both arm and x86:

```bash
docker buildx build --push --platform linux/arm64,linux/amd64 -t apax/vagrant-ubuntu:20.04 -f Dockerfile.focal .
```