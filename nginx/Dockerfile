FROM nginx:alpine

MAINTAINER David Yang <yangyulin629@163.com>

ADD nginx.conf /etc/nginx/

RUN apk update \
    && apk upgrade \
    && apk add --no-cache bash \
    && adduser -D -H -u 1000 -s /bin/bash www-data


CMD ["nginx"]

EXPOSE 80 443