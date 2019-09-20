FROM php:5.6-apache    #このdockerイメージを使います
COPY php.ini /usr/local/etc/php/
#hostにある php.iniファイルを　コンテナの中の  /usr/local/etc/php/にコピーしていきます

#下記の命令を実行します。いくつか必要なパッケージをインストールします。
RUN apt-get update \
  && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng-dev libmcrypt-dev \
  && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv mcrypt
