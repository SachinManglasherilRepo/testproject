
create a EC2 instance  and check the status till everycheck is completed.

Go to Downloads folder and connect via ssh

apt-get update

apt-get install apache2 -y

sudo apt-get install php

php -v

sudo apt-get install php8.3-cli php8.3-common php8.3-curl php8.3-gd php8.3-json php8.3-mbstring php8.3-intl php8.3-mysql php8.3-xml php8.3-zip
----------------------------------------------------

sudo apt-get install mysql-server

sudo mysql_secure_installation

sudo mysql

mysql> ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'admin12345';
FLUSH PRIVILEGES;

mysql -u root -p 
password

to enter to mysql 

CREATE DATABASE dbname;
SHOW DATABASES;

-----------------------------------------------
$ php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
$ php -r "if (hash_file('sha384', 'composer-setup.php') === 'e0012edf3e80b6978849f5eff0d4b4e4c79ff1609dd1e613307e16318854d24ae64f26d17af3ef0bf7cfb710ca74755a') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
$ php composer-setup.php
$ php composer-setup.php --install-dir=bin --filename=composer
$ php -r "unlink('composer-setup.php');"
$ composer --version


-------------------------

if facing issue with vendor folder ,remove it and  run composer install 

composer update --no-scripts
rm -rf bootstrap/cache/*.php

