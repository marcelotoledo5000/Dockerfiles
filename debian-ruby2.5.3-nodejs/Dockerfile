# To USE: skygvinn/debian-ruby-nodejs:v1.3

FROM ruby:2.5.3

LABEL name="Debian-Ruby2.5.3-NodeJS" \
  version="1.3"

RUN apt-get update -y && \
  gem update --system && \
  gem install bundler && \
  apt-get install curl software-properties-common -y && \
  curl -sL https://deb.nodesource.com/setup_10.x | bash - && \
  apt-get install apt-utils nodejs -y && \
  gem cleanup && \
  apt-get clean
