FROM debian:latest

MAINTAINER dailytechlearning

RUN apt-get update && apt-get install -y apache2 && apt-get clean && rm -rf /var/lib/apt/lists/*

ENV APACHE_USER www-data
ENV APACHE_GRP  www-data
ENV APACHE_LOG /var/log/apache2


EXPOSE 80

CMD ["usr/bin/apache2", "-D", "FOREGROUND"]
