FROM ubuntu:16.04

RUN apt-get -y update
RUN apt-get -y install git libpq-dev postgresql-client curl
RUN apt-get -y install ruby-dev
RUN gem install bundler
RUN gem install capistrano -v 3.7.2
RUN gem install capistrano-composer
RUN apt-get -y install php7.0 \
    php7.0-opcache \
    php7.0-fpm \
    php7.0-xml \
    php7.0-pdo \
    php7.0-mbstring \
    php7.0-pgsql \
    php7.0-curl \
    php7.0-bcmath \
    phpunit \
    php-apcu

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin/ --filename=composer

WORKDIR "/code"
