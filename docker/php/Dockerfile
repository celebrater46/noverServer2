FROM php:7.4-apache

RUN apt-get update \
    && apt-get install -y libonig-dev \
    libzip-dev \
    unzip \
    mariadb-client \
    && docker-php-ext-install pdo_mysql \
    mysqli \
    mbstring \
    zip

WORKDIR /var/www/html

EXPOSE 80