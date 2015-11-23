FROM ubuntu:latest
MAINTAINER Ivan <ivanpetrus@gmail.com>

RUN apt-get update && apt-get install -y software-properties-common

RUN locale-gen en_US.UTF-8 
ENV LANG en_US.UTF-8

RUN apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_5.x | sudo -E bash -


RUN apt-get install -y nodejs build-essential

WORKDIR /app
