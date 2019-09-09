#This is dockerfile for mycart MS frontend layer
FROM centos:7
MAINTAINER rahulr.uvce@gmail.com
RUN yum -y update
RUN yum -y install httpd php php-gd php-mysql
ADD code /var/www/html
EXPOSE 80
ENV MY_DB_HOST_WRITE=test MY_DB_NAME=test MY_DB_USER=test MY_DB_PASS=test MY_DB_HOST_READ=test

ADD scripts /usr/bin/
RUN chmod 755  /usr/bin/startapache
CMD ["startapache"]