#FROM nginx:latest
FROM nginx:alpine

LABEL maintainer="Manjunath Muniraju <mmuniraju4444@gmail.com>"

ADD ./conf/nginx.conf /etc/nginx/

ADD ./conf/app.conf /etc/nginx/sites-available/app.conf

#RUN apt-get update

RUN rm /etc/nginx/conf.d/default.conf

STOPSIGNAL SIGTERM

CMD ["nginx"]

