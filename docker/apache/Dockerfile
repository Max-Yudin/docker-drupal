FROM ubuntu:latest

RUN apt-get update \
    && echo "mysql-server mysql-server/root_password password 111" | debconf-set-selections \
    && echo "mysql-server mysql-server/root_password_again password 111" | debconf-set-selections \
    && apt-get install -y \
    net-tools \
    vim \
    mc \
    git \
    drush \
    nginx \
    mysql-server \
    php-fpm \
    php-cli \
    php-curl \
    php-gd \
    php-json \
    php-mysql \
    php-xml \
    php-intl \
    php-mbstring \
    php-zip

RUN mkdir -p /var/www/drupal/
RUN mkdir -p /var/www/html/sites/default/files/ && chmod 777 -R /var/www/html/sites/default/files/
