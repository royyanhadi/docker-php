FROM royyanhadi/php:5.6-apache
MAINTAINER Royyan Hadi Sunyoto<royyan.sunyoto@pelindo.co.id>

RUN a2enmod rewrite headers
COPY ./config/apache2.conf ${APACHE_CONFDIR}/apache2.conf
COPY ./config/app-config.conf ${APACHE_CONFDIR}/sites-enabled/app-config.conf

COPY ./app /var/www/html/