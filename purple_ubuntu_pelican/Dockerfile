###
from ubuntu:18.04

LABEL maintainer="purple cabbage"
LABEL VERSION="1.0" ARCHITECTURE="amd64"

RUN apt update && \
 apt -y install python3 \
                python3-pip \
                python3-venv  \
                git \
                vim   
                 


RUN adduser --disabled-password --gecos ""  purple
USER purple

RUN cd $HOME && \
    mkdir -p  PDevWS/purpleblog && \
    cd PDevWS/purpleblog  && \
    python3 -m venv devenv && \
    cd devenv && \
    . ./bin/activate  && \
    pip install markdown wheel && \
    pip install pelican
    

CMD ["/bin/bash"]

