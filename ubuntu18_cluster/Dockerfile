FROM ubuntu:18.04

RUN apt-get update && apt-get install -y init && apt-get clean all
RUN apt-get -y update
RUN apt-get install -y gcc
RUN apt-get install -y vim
RUN apt-get install -y net-tools
RUN apt-get install -y openjdk-8-jdk
RUN apt-get install ssh -y
RUN apt-get install openssh-server -y
RUN echo "PermitRootLogin yes" >> /etc/ssh/sshd_config
RUN service ssh start
RUN cd /root
RUN wget https://archive.apache.org/dist/hadoop/core/hadoop-1.2.1/hadoop-1.2.1-bin.tar.gz
RUN tar -xvzf hadoop-1.2.1-bin.tar.gz


EXPOSE 22

