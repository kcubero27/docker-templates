FROM php:fpm-alpine

RUN apk update

RUN apk add --no-cache $PHPIZE_DEPS \
    && pecl install xdebug \
	&& docker-php-ext-enable xdebug

CMD ["php-fpm"]

EXPOSE 9000