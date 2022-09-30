FROM  ubuntu
RUN  apt update -y
RUN  apt install apache2 -y
RUN  apt install php8.1 -y
RUN  apt install libapache2-mod-php8.1  -y
RUN  apt  install php8.1-mysqli  -y
RUN  systemctl reload apache2
COPY . /var/www/html
