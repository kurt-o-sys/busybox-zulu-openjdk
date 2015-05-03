# zulu-openjdk

Dockerfile for a minimal free jdk. It uses busybox as tiny linux distro and Azul zulu as jdk. The code is taken from peelsky/zulu-openjdk-busybox, but this one includes 8u40. For previous versions, please refer to [peelsky/zulu-openjdk-busybox](https://registry.hub.docker.com/u/peelsky/zulu-openjdk-busybox/). For a minimal (Oracle) jre only, check out [cloudunder/java-runtime](https://registry.hub.docker.com/u/cloudunder/java-runtime/).

## Image sizes

As a comparison:

```
name                           tag                size  
peelsky/zulu-openjdk-busybox   6u56               148.3 MB
peelsky/zulu-openjdk-busybox   6                  148.3 MB

cloudunder/java-runtime        7                  123.5 MB
cloudunder/java-runtime        latest             123.5 MB
peelsky/zulu-openjdk-busybox   7                  160.9 MB
peelsky/zulu-openjdk-busybox   7u72               160.9 MB
java                           openjdk-7-jre      332.3 MB
dockerfile/java                openjdk-7-jre      684.4 MB

peelsky/zulu-openjdk-busybox   8                  181.8 MB
peelsky/zulu-openjdk-busybox   8u25               181.8 MB
peelsky/zulu-openjdk-busybox   latest             181.8 MB
simplexsys/zulu-openjdk        8u40               182.8 MB
```


## Usage

docker run -it --rm simplexsys/zulu-openjdk:8u40 java -version
docker run -it --rm simplexsys/zulu-openjdk:latest java -version
