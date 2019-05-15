FROM php:7.1-fpm
#将源 传入
ADD source.list /root/source.list
#RUN ~/source.list >> /etc/apt/sources.list
#安装pdo_mysql 其他插件也可以通过docker-php-ext-install的方式安装
RUN apt-get update && apt-get install -y \
&& docker-php-ext-install pdo_mysql        
EXPOSE 9000

