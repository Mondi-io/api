# Mondi API

This is the dockerized API repo for Mondi.

## Purpose

The purpose of having this layer is to be able to interact with other APIs through this layer
and make this layer the data producer to the Kafka broker.

## Quick Note

New API's will be added under src/

## Quick Docker Instructions

[https://nodejs.org/en/docs/guides/nodejs-docker-webapp/]

### To build

```
$ docker build -t <image_tag>
```

### To run

Running your image with -d runs the container in detached mode, leaving the container running in the background. The -p flag redirects a public port to a private port inside the container.

```
docker run -p 49160:8080 -d <image_tag>
```

### To check docker images

```
$ docker images
```

### To check what is running in docker

```
$ docker ps
```

### To print the output

```
docker logs <container id>
```

### To enter the container
```
docker exec -it <container id> /bin/bash
```
