FROM ubuntu:18.04

RUN apt update 

RUN apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates

RUN curl -sL https://deb.nodesource.com/setup_12.x |  bash -

RUN apt install -y nodejs \
    gcc \
    g++ \
    make \
    python3-pip \
 && pip3 install \
    awscli


# FROM node:12.16.1

# RUN apt update 

# RUN apt install -y jq \
#     git \
#     yarn \ 
#     gcc \ 
#     g++ \
#     make \
#     python3-pip \
#     && pip3 install \
#     awscli
   
