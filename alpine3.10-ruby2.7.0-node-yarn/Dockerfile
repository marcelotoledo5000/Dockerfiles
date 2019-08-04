# TO USE: skygvinn/alpine-ruby2.7-node-yarn:v1.0

FROM 2.7.0-preview1-alpine3.10

LABEL name="Alpine-Ruby-2.7-Node-Yarn" \
  version="1.0"

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
