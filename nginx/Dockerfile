FROM nginx:alpine

MAINTAINER Starriv <starriv.993@gmail.com>

ADD nginx.conf /etc/nginx/
COPY vhost/*.conf /etc/nginx/sites-available/

ARG PHP_UPSTREAM=php-fpm

RUN apk update \
    && apk upgrade \
    && apk add --no-cache bash \
    && adduser -D -H -u 1000 -s /bin/bash www-data \
    && rm /etc/nginx/conf.d/default.conf \
#    && echo "upstream php-upstream { server ${PHP_UPSTREAM}:9000; }" > /etc/nginx/conf.d/upstream.conf
    && echo "upstream php-upstream { server ${PHP_UPSTREAM}:9000; }" > /etc/nginx/nginx.conf

CMD ["nginx"]
EXPOSE 80
