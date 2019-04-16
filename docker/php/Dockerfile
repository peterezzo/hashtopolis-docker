ARG PHP_VERSION=""
FROM php:${PHP_VERSION:+${PHP_VERSION}-}fpm

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    libpng-dev \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install gd mysqli pdo_mysql

COPY php.ini /usr/local/etc/php-fpm.d/z-hashtopolis.conf