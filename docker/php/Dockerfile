FROM php:8.4-fpm-alpine

RUN apk update

RUN apk add \
    php-curl \
    php-xml \
    php-intl \
    php-xdebug \
    php-mbstring
    
RUN docker-php-ext-install mysqli pdo pdo_mysql && docker-php-ext-enable pdo_mysql