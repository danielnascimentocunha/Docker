FROM ubuntu:20.04
MAINTAINER dnemo
ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update
RUN apt-get install apache2 -y
RUN apt-get clean
COPY index.html /var/www/html
CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]
EXPOSE 80
