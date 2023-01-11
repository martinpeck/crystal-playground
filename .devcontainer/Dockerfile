FROM mcr.microsoft.com/devcontainers/base:jammy

# This will be set to true when running in VSCode
ARG INTERACTIVE="false"
ARG USERNAME=vscode
ARG USER_UID=1000
ARG USER_GID=$USER_UID

RUN apt-get update && apt-get install -y curl \
                                         build-essential \
                                         gnupg \
                                         ca-certificates \
                                         apt-transport-https \
                                         libssl-dev \
                                         libxml2-dev \
                                         libyaml-dev \
                                         libgmp-dev \
                                         libz-dev \
                                         libevent-dev \
                                         pkgconf \
                                         --no-install-recommends \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*
    
USER $USERNAME
