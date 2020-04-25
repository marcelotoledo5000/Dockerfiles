# TO USE: skygvinn/alpine3-ruby2.7-nodejs:v1.1

FROM ruby:2.7-alpine3.11

LABEL name="Alpine3-Ruby-2.7-Node-Yarn" \
  version="1.1"

RUN apk add --update --no-cache \
  build-base \
  bash \
  cmake \
  coreutils \
  git \
  nodejs \
  postgresql-dev \
  yarn \
  tzdata && \
  gem update --system && \
  gem install bundler && \
  gem cleanup
