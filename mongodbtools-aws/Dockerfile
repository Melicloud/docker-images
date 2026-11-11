FROM debian:13.7

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update && \
    apt install wget awscli \ 
    nano telnet apt-transport-https ca-certificates curl \
    gnupg-agent unzip less -y && \
    wget https://fastdl.mongodb.org/tools/db/mongodb-database-tools-debian13-x86_64-100.20.1.deb && apt install ./mongodb-database-tools-*-100.20.1.deb && rm ./mongodb-database-tools-*-100.20.1.deb && \
    apt clean && \
    rm -rf /var/lib/apt/lists/*
