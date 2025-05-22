FROM php:8.2-apache

RUN apt-get update && apt-get install -y \
    libpq-dev \
    && docker-php-ext-install pdo pdo_pgsql

# ドキュメントルートの権限などを調整する場合
RUN chown -R www-data:www-data /var/www/html
