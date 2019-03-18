# TO USE: skygvinn/debian-ruby2.6-mariadb:v1.0

FROM ruby:2.6.0

LABEL name="Debian-Ruby-2.6-NodeJS-MariaDB" \
      version="1.0"

RUN apt-get update && \
    apt-get install devscripts \
    dh-make \
    libmariadbclient-dev \
    libxml2-dev \
    cmake \
    pkg-config \
    libdistro-info-perl -y && \
    apt-get clean

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash - && \
    apt-get install apt-utils nodejs -y && \
    apt-get install curl software-properties-common -y && \
    apt-get install tzdata -y && \
    gem update --system && \
    gem install bundler && \
    gem cleanup && \
    apt-get clean
