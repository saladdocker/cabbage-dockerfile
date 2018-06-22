###
from centos:7

LABEL maintainer="purple cabbage"
LABEL VERSION="1.0" ARCHITECTURE="amd64"

RUN yum -y update && \
 yum -y install https://centos7.iuscommunity.org/ius-release.rpm  && \
 rpm --import /etc/pki/rpm-gpg/IUS-COMMUNITY-GPG-KEY && \
 yum -y install gcc gcc-c++ cmake make git2u  && \
 yum clean all


RUN useradd purple

USER purple

CMD ["/bin/bash"]

