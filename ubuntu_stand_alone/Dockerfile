FROM ubuntu:18.04

ADD ./hadoop-2.7.2.tar.gz /

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
# RUN cd /root
# RUN tar -xvzf hadoop-2.7.2.tar.gz
# RUN rm hadoop-2.7.2.tar.gz
# RUN mv hadoop-2.7.2 ./root/


EXPOSE 22

