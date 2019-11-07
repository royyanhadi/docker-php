FROM royyanhadi/php:7.0-fpm

MAINTAINER Royyan Hadi Sunyoto<royyan.sunyoto@pelindo.co.id>

ADD nginx/nginx.conf /etc/nginx/nginx.conf
ADD nginx/fastcgi_params /etc/nginx/fastcgi_params
ADD nginx/default /etc/nginx/sites-enabled/default

ADD php-fpm/www.conf /usr/local/etc/php-fpm.d/www.conf
ADD php-fpm/php.ini /usr/local/etc/php/php.ini

ADD app /app
RUN chown -R www-data:www-data /app

ADD start.sh /
RUN chmod +x /start.sh
CMD /start.sh