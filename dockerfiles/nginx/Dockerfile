FROM debian:stretch
RUN apt-get update && apt-get install -y nginx vim nano

ADD ./conf/nginx/sites-enabled /etc/nginx/sites-enabled
RUN rm /etc/nginx/sites-enabled/default
WORKDIR /usr/share/nginx/html/app

EXPOSE 80
EXPOSE 443

CMD ["nginx"]