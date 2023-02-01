FROM php:7.4.14-fpm

# Set working directory
WORKDIR /var/www
#
RUN usermod -u 1000 www-data && groupmod -g 1000 www-data

#
RUN mkdir -p /var/www/biodata/logs && chmod 777 /var/www/biodata/logs
#
CMD /etc/init.d/cron start && php-fpm