#This is dockerfile for mycart MS frontend layer
FROM centos:7
MAINTAINER rahulr.uvce@gmail.com
RUN yum -y update
RUN yum -y install httpd php php-gd
ADD code /var/www/html
EXPOSE 80
ENV BACKENDLB=test
ADD scripts /usr/bin/
RUN chmod 755  /usr/bin/startapache
CMD ["startapache"]