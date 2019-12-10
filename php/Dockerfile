FROM php:7.2.2-fpm
RUN apt-get update
RUN /usr/local/bin/docker-php-ext-install opcache 
RUN pecl install yaf
RUN pecl install redis
RUN /usr/local/bin/docker-php-ext-enable opcache yaf redis 
RUN apt-get update -y
RUN apt-get install -y libfreetype6-dev libmcrypt-dev libjpeg-dev libpng-dev
RUN docker-php-ext-configure gd --enable-gd-native-ttf --with-freetype-dir=/usr/include/freetype2 --with-png-dir=/usr/include --with-jpeg-dir=/usr/include
RUN docker-php-ext-install gd pdo pdo_mysql mysqli