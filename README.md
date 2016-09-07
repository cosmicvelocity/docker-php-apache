# docker-php-apache

[php:5.6.25-apache](https://hub.docker.com/_/php/) をカスタマイズした docker イメージです。

下記のモジュールが追加されています。

- curl
- gd
- intl
- imagick (3.4.1)
- mbstring
- mcrypt
- memcached (2.2.0)
- pdo_mysql
- redis (2.2.8)
- swfed (0.64)

## 例

    $ docker run -v $(pwd)/examples:/var/www/html -p 80:80 --name php-apache --rm cosmicvelocity/php:5.6.25-apache

## ドキュメント

### コンテナのビルド

    git clone https://github.com/cosmicvelocity/docker-php-apache.git
    cd docker-php-apache
    git checkout 5.6.25
    cd 5.6.25
    docker build -t cosmicvelocity/php:5.6.25-apache .

### 実行

    $ docker run -v $(pwd)/examples:/var/www/html -p 80:80 --name php-apache --rm cosmicvelocity/php:5.6.25-apache
