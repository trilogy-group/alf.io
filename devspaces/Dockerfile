FROM postgres:10

LABEL description="Devspaces base implementation for alfio"

RUN apt-get update \
 && apt-get install --assume-yes apt-utils \
 software-properties-common \
 dconf-cli \
 unzip \
 wget \
 openjdk-8-jdk \
 fontconfig && apt-get clean

WORKDIR /data
ENV ALFIO_LOG_STDOUT_ONLY=true
ENV ALFIO_JAVA_OPTS=""
