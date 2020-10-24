# docker-php-xdebug-nginx

Based on [Shana's Article](https://x-team.com/blog/docker-compose-php-environment-from-scratch/).

## Installation
```
$ docker-compose up --build
```

## Tips
Check xDebug version:
```
$ docker exec -it docker_php-fpm_1 /bin/sh  
$ php -i | grep Xdebug
with Xdebug v2.9.8, Copyright (c) 2002-2020, by Derick Rethans
Support Xdebug on Patreon, GitHub, or as a business: https://xdebug.org/support
```

## PHPStorm Xdebug 

