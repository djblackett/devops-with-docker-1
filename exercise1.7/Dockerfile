FROM ubuntu:20.04

WORKDIR /usr/src/app

RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install -y curl

COPY curl.sh .

ENTRYPOINT ["./curl.sh"]
