FROM php:7.0-apache
COPY php.ini /usr/local/etc/php/
RUN apt-get update && \
  docker-php-ext-install pdo_mysql mysqli mbstring