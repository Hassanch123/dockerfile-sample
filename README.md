# dockerfile-sample

FROM ubuntu:16.04

MAINTAINER Hassan

RUN apt-get update
Run apt-get install -y python3 python3-pip
COPY. /app
WORKDIR /app

EXPOSE 5000

ENTRYPOINT echo "Hello World !"
