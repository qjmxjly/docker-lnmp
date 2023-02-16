######
# See: https://hub.docker.com/_/php/
######

FROM php:7-fpm
MAINTAINER micooz <micooz@hotmail.com>

######
# You can install php extensions using docker-php-ext-install
#####
RUN curl -sSLf \
        -o /usr/local/bin/install-php-extensions \
        https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions && \
    chmod +x /usr/local/bin/install-php-extensions && \
    install-php-extensions gd pdo_mysql mysqli && \
    apt update && \
    apt install python -y
