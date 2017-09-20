# a tiny Docker container of a smallest "Hello Docker World App"

[![](https://dronehub.dev.sys3.org/api/badges/curx/hello-docker-world/status.svg)](https://dronehub.dev.sys3.org/api/badges/curx/hello-docker-world/status.svg)
[![](https://images.microbadger.com/badges/image/curx/hello-docker-world.svg)](https://microbadger.com/images/curx/hello-docker-world "Get your own image badge on microbadger.com")

This example demonstrates the use of [Docker multi-stage builds](https://docs.docker.com/engine/userguide/eng-image/multistage-build/) to create a smallest "Hello Docker World" container. The resulting docker container is only `512 Byte`, compared to `156 MB` of full `alpine:latest` alpine base image with build environment.

It is used for testing and training.

## Build the hello-docker-world app

**Note:** You will need docker a version higher or equal to 17.05 use the multistate build.

```
docker build -t hello-docker-world .
```

## Run the container

```
docker run --ti --rm hello-docker-world
```
