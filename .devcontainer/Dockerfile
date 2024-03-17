FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

# Install essential tools.
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    make \
    curl \
    git-all \
    python3 \
    python3-pip \
    sudo \
    wget \
    && rm -rf /var/lib/apt/lists/* \
    && rm -Rf /usr/share/doc && rm -Rf /usr/share/man \
    && apt-get clean

RUN curl -sf -L https://download.daytona.io/daytona/get-server.sh | sudo bash

USER ${USERNAME}

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt