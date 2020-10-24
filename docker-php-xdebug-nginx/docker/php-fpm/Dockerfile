FROM php:fpm-alpine

# install xdebug
RUN apk add --no-cache $PHPIZE_DEPS \
    && pecl install xdebug \
	&& docker-php-ext-enable xdebug

CMD ["php-fpm"]

EXPOSE 9000