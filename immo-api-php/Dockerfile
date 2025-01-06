FROM php:8.1-apache

RUN apt-get update && apt-get install -y \
    git \
    unzip \
    zip \
    && docker-php-ext-install zip

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN php -m | grep zip
RUN composer --version

COPY . /var/www/html/

EXPOSE 80

CMD ["apache2-foreground"]
