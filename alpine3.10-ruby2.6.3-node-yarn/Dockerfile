# TO USE: skygvinn/alpine-ruby2.6-nodejs:v1.2

FROM ruby:2.6.3-alpine3.10

LABEL name="Alpine3.10-Ruby-2.6-Node-Yarn" \
  version="1.2"

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
