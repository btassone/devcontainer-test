ARG VARIANT=latest
FROM ubuntu:${VARIANT}

ARG USERNAME=app
ARG USER_UID=1000
ARG USER_GID=$USER_UID

RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends curl ca-certificates nginx zsh \
    && apt-get autoremove -y \
    && apt-get clean -y
