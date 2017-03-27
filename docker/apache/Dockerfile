FROM ubuntu:latest

RUN apt-get update \
    && apt-get install -y apache2 \
    drush \
    php-cli \
    php-curl \
    php-gd \
    php-json \
    php-mysql \
    php-xml \
    php-fpm \
    php-intl \
    php-mbstring \
    php-zip \
    libapache2-mod-php \
    && a2enmod rewrite

RUN mkdir -p /var/www/html/sites/default/files/ && chmod 777 -R /var/www/html/sites/default/files/

EXPOSE 80

CMD ["apachectl", "-D", "FOREGROUND"]