FROM php:8.4-fpm-alpine


# mv "/usr/local/etc/php/php.ini-production" "/usr/local/etc/php/php.ini"   
# RUN mv "$PHP_INI_DIR/php.ini-production" "$PHP_INI_DIR/php.ini"

COPY docker/php/config/php.ini "$PHP_INI_DIR/php.ini"

RUN apk update

# RUN apk add \
#     php-intl \
#     php-xdebug \
    
RUN docker-php-ext-install mysqli pdo pdo_mysql && docker-php-ext-enable pdo_mysql