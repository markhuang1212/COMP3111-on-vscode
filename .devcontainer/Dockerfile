FROM ubuntu:rolling

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install git build-essential sudo apt-utils ca-certificates gnupg

RUN update-ca-certificates

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install openjdk-15-jdk

RUN useradd -ms /bin/bash -G sudo vscode
RUN echo "vscode ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers.d/vscode
RUN chmod 0440 /etc/sudoers.d/vscode

USER vscode