FROM wordpress:5.9.0-php7.4-apache
#RUN ln -s /usr/local/lib/php/extensions/no-debug-non-zts-20190902/ /usr/local/lib/php/extensions/no-debug-non-zts-20170718
RUN pecl install xdebug-3.1.3 && docker-php-ext-enable xdebug
