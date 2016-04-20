FROM ubuntu:latest
MAINTAINER Ivan <ivan@marsud.id>

RUN apt-get update && apt-get install -y software-properties-common

RUN locale-gen en_US.UTF-8
ENV LANG en_US.UTF-8

RUN echo Node 5.10.1 && \
    apt-get update && \
    apt-get install -y curl && \
    curl -sL https://deb.nodesource.com/setup_5.x | sudo -E bash -

RUN apt-get install -y nodejs python build-essential git && apt-get autoclean

RUN npm install -g bower gulp phantomjs eslint node-gyp

WORKDIR /app
