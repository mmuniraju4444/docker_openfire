FROM httpd:2.4.33-alpine

RUN addgroup -S app && adduser -S -G app app
COPY Config/httpd.conf /usr/local/apache2/conf/httpd.conf