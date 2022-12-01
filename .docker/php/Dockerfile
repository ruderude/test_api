FROM php:8.1-fpm

WORKDIR /var/www/html

RUN apt-get update
RUN apt-get install -y build-essential libpq-dev git curl unzip

RUN docker-php-ext-install pdo_pgsql pcntl

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
