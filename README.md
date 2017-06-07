# develop

### php7
$ yum install epel-release
$ rpm -Uvh http://rpms.famillecollet.com/enterprise/remi-release-7.rpm
$ curl -L https://raw.github.com/CHH/phpenv/master/bin/phpenv-install.sh | bash

$ git clone git://github.com/CHH/php-build.git ~/.phpenv/plugins/php-build

$ cd .phpenv/plugins/php-build/
$ sh install.sh

$ echo 'export PATH="$HOME/.phpenv/bin:$HOME/.phpenv/versions/7.0.0RC5/sbin:$PATH"' >> ~/.bashrc

$ echo 'eval "$(phpenv init -)"' >> ~/.bashrc


$ exec $SHELL -l

$ yum install libxml2-devel bison bison-devel openssl-devel curl-devel libjpeg-devel libpng-devel libmcrypt-devel readline-devel libtidy-devel libxslt-devel





$ wget -P /usr/share/ https://sourceforge.net/projects/re2c/files/0.14.3/re2c-0.14.3.tar.gz


$ tar zxvf re2c-0.14.3.tar.gz -C /usr/share/
$ cd re2c-0.14.3

$ ./configure
$ make install

バージョン確認
$ php-build --definitions

PHPインストール
$ php-build 5.6.30 ~/.phpenv/versions/5.6.30


$ phpenv versions

$ phpenv global 7.0.19
$ phpenv rehash
$ php -v
PHP 7.0.19 (cli) (built: Jun  3 2017 23:38:13) ( NTS )
Copyright (c) 1997-2017 The PHP Group
Zend Engine v3.0.0, Copyright (c) 1998-2017 Zend Technologies
    with Zend OPcache v7.0.19, Copyright (c) 1999-2017, by Zend Technologies
    with Xdebug v2.5.3, Copyright (c) 2002-2017, by Derick Rethans


#### For git
$ git init
$ git add README.md
$ git commit -m "First Commit"
$ git remote add origin git@github:*****/****.git
$ git push -u origin master


### composer のダウンロード
$ curl -sS https://getcomposer.org/installer | php
[root@2d72f776a1b6 cetntos]# mv composer.phar /usr/local/bin/composer
[root@2d72f776a1b6 cetntos]# chmod +x /usr/local/bin/composer


### Laravel のインストール
[root@2d72f776a1b6 cetntos]# composer global require "laravel/installer"
[root@2d72f776a1b6 cetntos]# PATH=$PATH:~/.composer/vendor/bin


### Project の作成
$ laravel new dev01
