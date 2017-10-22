FROM php:7.1.10-fpm
RUN docker-php-ext-install pdo pdo_mysql && \
    curl -sS https://getcomposer.org/installer | php && \
    mv composer.phar /usr/local/bin/composer
