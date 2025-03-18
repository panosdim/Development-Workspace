FROM codercom/enterprise-base:ubuntu

USER root

RUN apt-get update \
    && apt-get install -y \
    sudo \
    curl \
    git \
    golang \
    vim \
    wget \
    && rm -rf /var/lib/apt/lists/*

ARG USER=coder
USER ${USER}
WORKDIR /home/${USER}
