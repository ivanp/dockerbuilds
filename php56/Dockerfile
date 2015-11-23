FROM ubuntu:latest
MAINTAINER Ivan <ivanpetrus@gmail.com>

RUN apt-get update && apt-get install -y software-properties-common

RUN locale-gen en_US.UTF-8 
ENV LANG en_US.UTF-8

RUN add-apt-repository -y ppa:ondrej/php5-5.6 

RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 4F4EA0AAE5267A6C

RUN apt-get update && apt-get install -y \
	php5-cli php5-common php5-curl php5-fpm php5-gd php5-mcrypt php5-mysql php5-pgsql php5-sqlite php5-readline php5-redis php5-xdebug php5-mongo 

    
ADD php-fpm.conf /etc/php5/fpm/php-fpm.conf

CMD ["php5-fpm", "-F"]