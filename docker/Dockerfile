#
# Alf.io dockerfile.
#

# Pull base image.
FROM openjdk:8-jdk-stretch

RUN useradd -ms /bin/bash -u 1001 alfio
RUN apt-get update \
 && apt-get install --assume-yes apt-utils \
 software-properties-common \
 dconf-cli \
 unzip \
 wget \
 fontconfig

USER alfio

# Define working directory.
WORKDIR /home/alfio
RUN mkdir /home/alfio/logs
ENV ALFIO_LOG_STDOUT_ONLY=true
ENV ALFIO_JAVA_OPTS=""

CMD tail -f /dev/null