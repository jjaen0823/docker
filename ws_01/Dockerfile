FROM ubuntu:18.04

RUN apt-get update 
RUN apt-get install -y apache2

COPY ./hello.html /var/www/html
# == ADD ./hello.html /var/www/html

WORKDIR /var/www/html

# apache defaule service port number
EXPOSE 80

CMD [ "apachectl", "-DFOREGROUND" ] 
# CMD apachectl -DFOREGROUND 
# CMD [ "apachectl", "start", "-D", "FOREGROUND" ] 