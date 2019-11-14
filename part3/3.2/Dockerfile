FROM ubuntu:16.04

RUN apt-get update && apt-get install -y python3-pip ffmpeg wget && \
    pip3 install yle-dl && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /yle
ENTRYPOINT [ "yle-dl" ]
