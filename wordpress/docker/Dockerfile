FROM php:8.1-fpm

WORKDIR /usr/share/nginx/html

RUN apt-get update \
    && apt-get upgrade -y
RUN apt-get install wget
RUN wget https://wordpress.org/latest.tar.gz && tar xvfz latest.tar.gz && mv wordpress/* ./ && rmdir wordpress

RUN docker-php-ext-install mysqli pdo pdo_mysql
