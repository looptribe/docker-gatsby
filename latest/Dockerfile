FROM node

MAINTAINER Claudio Gandelli <claudio.gandelli@looptribe.com>

RUN apt-get update && apt-get install -y \
    gettext-base \
    rsync \
    lftp

RUN npm install -g gatsby-cli

RUN mkdir /data && chown node:node /data

VOLUME /data
WORKDIR /data