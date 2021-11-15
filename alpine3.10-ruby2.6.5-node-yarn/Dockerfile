# TO USE: skygvinn/alpine-ruby2.6.5-nodejs:v1.3

FROM ruby:2.6-alpine3

LABEL name="Alpine3-Ruby-2.6-Node-Yarn" \
      version="1.4"

RUN apk add --update --no-cache \
    build-base \
    bash \
    coreutils \
    git \
    nodejs \
    postgresql-dev \
    yarn \
    tzdata && \
    gem update --system && \
    gem install bundler && \
    gem cleanup
