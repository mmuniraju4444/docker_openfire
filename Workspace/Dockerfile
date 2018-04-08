FROM  php:7.2.4-cli-alpine3.7

WORKDIR /var/www/html

RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
php composer-setup.php --install-dir=/usr/bin --filename=composer && \
php -r "unlink('composer-setup.php');"

RUN addgroup -S app && adduser -S -G app app