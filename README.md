# Alpine-based ERDDAP images
In this repo you will find minimal ERDDAP images.

## Docker Hub
The public docker hub repository is here: https://hub.docker.com/r/lloydcotten/alpine-erddap/

Images are built from `lloydcotten/alpine-tomcat:8-jre8`.

## Usage
```
CID=$(docker run -it --rm lloydcotten/alpine-erddap:v1.68)
docker inspect --format '{{ .NetworkSettings.IPAddress }}' "${CID}"
```
Visit http://*<IPAddress>*:8080/ in a web browser on your host machine.


## Images

* ERDDAP 1.68: `docker pull lloydcotten/alpine-erddap:v1.68`
