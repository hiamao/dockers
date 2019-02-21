FROM ruby:2.6.1-alpine

ENV RUNTIME_PACKAGES="libxml2-dev libxslt-dev libstdc++ tzdata mariadb mariadb-client ca-certificates"\
    DEV_PACKAGES="build-base mariadb-dev"

RUN apk add --update --no-cache $RUNTIME_PACKAGES &&\
    apk add --update\
    --virtual build-dependencies\
    --no-cache\
    $DEV_PACKAGES &&\
    gem install bundler
