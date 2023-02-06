# syntax=docker/dockerfile:1
# hadolint ignore=DL3018

FROM alpine:3.17
LABEL org.opencontainers.image.source=https://github.com/roalcantara/dockers
LABEL org.opencontainers.image.description="Lua dev env based on Alpine linux"
LABEL org.opencontainers.image.licenses=MIT

RUN echo "@testing http://nl.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories \
  && apk -U --no-cache add lua lua-dev lua-doc lua-term lua-penlight lua-busted lua-luassert lua-inspect lua-lpeg-dev lua-filesystem lua-alt-getopt moonscript \
  && rm -rf /tmp/* /etc/apk/cache/*
