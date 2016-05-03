FROM debian:jessie

MAINTAINER Agnaldo Marinho <agnaldoneto@ufpa.br>

# Install Apache2 / PHP 5
RUN apt-get update && apt-get -y install apache2 php5 libapache2-mod-php5 php5-mysql php-pear php5-curl curl 

# Enable Apache2 modules
RUN a2enmod rewrite

# Set up the Apache2 environment Variables
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR  /var/log/apache2
ENV APACHE_LOCK_DIR /var/lock/apache2
ENV APACHE_PID_FILE /var/run/apache2.pid

EXPOSE 80


