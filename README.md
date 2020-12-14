# OpenDataPedia Docker repository

## Build

```shell
git clone https://github.com/opendatapedia/docker.git
cd docker/docker
VERSION=$(cat ../VERSION.txt) && docker build --build-arg VERSION -t opendatapedia:${VERSION} .
```

## Usage

```shell
docker run -it opendatapedia:0.0.1 sh
```