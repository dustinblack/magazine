FROM centos:7

USER root
RUN rpm -ivh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
RUN yum install -y java
RUN curl -O --location https://github.com/brianfrankcooper/YCSB/releases/download/0.15.0/ycsb-0.15.0.tar.gz
RUN mkdir ycsb
RUN tar xzf ycsb-0.15.0.tar.gz -C ycsb --strip-components 1
RUN yum install -y redis
RUN yum install -y python-elasticsearch
RUN yum install -y numpy
RUN yum install -y git
RUN git clone https://github.com/cloud-bulldozer/snafu /opt/snafu
