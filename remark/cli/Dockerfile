# syntax=docker/dockerfile:1
# hadolint ignore=DL3018

FROM node:lts-alpine
LABEL org.opencontainers.image.source=https://github.com/roalcantara/dockers
LABEL org.opencontainers.image.description="Remark cli based on Alpine linux"
LABEL org.opencontainers.image.licenses=MIT

RUN npm config set prefix /usr/local && npm install -g npm@latest && npm install -g remark-reference-links remark-cli
WORKDIR /app
ENTRYPOINT [ "/usr/local/bin/remark" ]
