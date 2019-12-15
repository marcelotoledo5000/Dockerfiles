# TO USE: skygvinn/alpine-ruby2.6.5-nodejs:v1.3

FROM ruby:2.6.5-alpine3.10

LABEL name="Alpine3.10-Ruby-2.6.5-Node-Yarn" \
  version="1.3"

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
