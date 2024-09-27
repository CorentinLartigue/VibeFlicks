# Dockerfile
FROM php:8.2-fpm

# Installer curl, git et les dépendances nécessaires pour les extensions PHP
RUN apt-get update && apt-get install -y \
    curl \
    git \
    libzip-dev \
    && docker-php-ext-configure zip --with-zip \
    && docker-php-ext-install zip \
    && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Installer l'extension pdo_mysql
RUN docker-php-ext-install pdo pdo_mysql

# Définir le répertoire de travail
WORKDIR /app

# Copier le code de l'application
COPY . /app  
