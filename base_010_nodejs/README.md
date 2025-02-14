# ETL Base 010 nodejs

This image provides generic functionality that is to be built upon.

Applications implementing this image have access to:
- nodejs

# Docker Image Development & Publication

## Build
```sh
docker build -t base_010_nodejs:develop -f ./Dockerfile .
```

## Run
```sh
docker run -it base_010_nodejs:develop
```

## Release
```sh
docker tag \
	base_010_nodejs:develop \
	base_010_nodejs:master

docker tag \
	base_010_nodejs:develop \
	base_010_nodejs:latest
```

## Publish
```sh
docker push base_010_nodejs:master
docker push base_010_nodejs:latest
```