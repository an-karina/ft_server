FROM	debian:buster

COPY	start.sh ./
RUN		apt-get -y upgrade && apt-get -y update
RUN		apt-get -y install nginx wordpress default-mysql-server php7.3 php7.3-fpm php-json php7.3-mysql php-mbstring openssl
# RUN		service nginx restart
CMD		bash start.sh
