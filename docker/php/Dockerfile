FROM ubuntu:latest

RUN apt-get update \
&&  apt-get -y install \
    libapache2-mod-php \
    php7.0 \
    php7.0-cli \
    php7.0-curl \
    php7.0-gd \
    php7.0-json \
    php7.0-mysql \
    php7.0-xml \
    php7.0-fpm \
    php7.0-intl \
    php7.0-mbstring \
    php7.0-zip

RUN mkdir -p /run/php/

CMD ["php-fpm7.0", "-F"]