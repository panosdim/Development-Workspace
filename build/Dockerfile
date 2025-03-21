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

# Install Node.js LTS
RUN curl -fsSL https://deb.nodesource.com/setup_lts.x | bash - \
    && apt-get install -y nodejs \
    && rm -rf /var/lib/apt/lists/*

ARG USER=coder
USER ${USER}
WORKDIR /home/${USER}
