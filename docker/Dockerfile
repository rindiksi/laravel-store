FROM php:8.3-fpm

# Install dependencies
RUN apt-get update && apt-get install -y \
    zip unzip curl git libzip-dev libonig-dev libxml2-dev \
    && docker-php-ext-install pdo pdo_mysql zip

# Install Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /var/www
