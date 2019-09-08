#Docker file for myapp runs in apache
FROM centos:7
MAINTAINER mailtoashish@gmail.com
RUN yum -y update
RUN yum -y install httpd
ADD code /var/www/html
EXPOSE 80
ENV BACKENDLB=test
CMD ["httpd", "-D" , "FOREGROUND"]