FROM php:fpm-alpine

RUN apk update

RUN apk add --no-cache $PHPIZE_DEPS

RUN pecl install xdebug \
    && docker-php-ext-enable xdebug

RUN docker-php-ext-install pdo pdo_mysql

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
    && composer --version

# Set timezone
# RUN rm /etc/localtime
# RUN ln -s /usr/share/zoneinfo/Europe/Berlin /etc/localtime
# RUN "date"

WORKDIR /var/www/