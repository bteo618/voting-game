# Playframework - Java for MyDOC
This file is intended to be host as a webpage itself and allow user to download the source code for the game.

## Installation
1. Put the zip file into *./conf/hostfile* folder and replace *download_source.gz* with the source file.

2. Create a docker image with:

```
export VERSION=1.0
export DOCKER_HOST=localhost
./build-docker-image.sh voting-monitor ${VERSION} ${DOCKER_HOST}
```

3. Run as docker:

```
docker run -p 9000:9000 -d localhost/voting-monitor:1.0
```

## Test
To test if this application can run correctly. run

```
#Unix
sbt run

#Windows
sbt.bat run
```
