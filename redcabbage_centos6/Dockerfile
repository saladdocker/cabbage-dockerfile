###
from centos:6

LABEL maintainer="Red Cabbage"
LABEL VERSION="1.0" ARCHITECTURE="amd64"

RUN yum -y update && \
 yum -y install https://centos6.iuscommunity.org/ius-release.rpm  && \
 rpm --import /etc/pki/rpm-gpg/IUS-COMMUNITY-GPG-KEY && \
 yum -y install gcc gcc-c++ cmake make git2u gdb vim  && \
 yum clean all


CMD ["/bin/bash"]

