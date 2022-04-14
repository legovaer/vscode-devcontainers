ARG FROM_REGISTRY=docker.pkg.github.com/legovaer/vscode-devcontainers
ARG FROM_IMAGE_NAME=commons-golang
ARG FROM_IMAGE_VERSION=latest
FROM ${FROM_REGISTRY}/${FROM_IMAGE_NAME}:${FROM_IMAGE_VERSION}

USER root

RUN apk add --update-cache \
  nodejs npm \
  && rm -rf /var/cache/apk/*

USER ${USERNAME}

