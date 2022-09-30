FROM  ubuntu
ARG DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y tzdata
RUN  apt update -y
RUN  apt install apache2 -y
RUN  apt install php8.1 -y
RUN  apt install libapache2-mod-php8.1  -y
RUN  apt  install php8.1-mysqli  -y
#RUN  systemctl start apache2
COPY . /var/www/html
RUN service apache2 restart
EXPOSE  80
CMD ["apache2ctl", "-D","FOREGROUND"]
