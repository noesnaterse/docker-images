FROM php:8.1-fpm

WORKDIR /usr/share/nginx/html

RUN apt-get update \
    && apt-get upgrade -y
RUN docker-php-ext-install mysqli pdo pdo_mysql
