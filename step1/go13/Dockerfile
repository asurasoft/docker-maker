FROM ubuntu:18.04
MAINTAINER Asurasoft <asurasoft@126.com>
COPY ./ali_sources.list /etc/apt/sources.list
RUN apt-get update
RUN apt-get -y install wget curl net-tools apt-utils
RUN wget https://dl.google.com/go/go1.13.5.linux-amd64.tar.gz
RUN tar -C /usr/local -xzf go1.13.5.linux-amd64.tar.gz
RUN echo "export GOPATH=/root/.go" >> /etc/profile
RUN echo "export PATH=$PATH:/usr/local/go/bin" >> /etc/profile
RUN echo "export GOPROXY=https://goproxy.cn,direct"
