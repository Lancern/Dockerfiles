FROM debian:stretch-slim

RUN apt-get --assume-yes update && \
    apt-get --assume-yes install apt-transport-https
COPY sources.list /etc/apt/sources.list
