## Use an Official Ubuntu Base Image
FROM ubuntu:latest

## Install Apache2
RUN apt-get -y update
RUN apt-get -y install apache2

## Copy index.html to Container
COPY ./web/index.html /var/www/html/

## Expose Port 80 on Container
EXPOSE 80

## Starts Apache2 Service When Container is Executed
CMD ["apache2ctl", "-D", "FOREGROUND"]