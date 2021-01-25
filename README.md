# CMS with Doctrine ORM and MVC architecture

A custom content management system created with raw PHP using Doctrine ORM, Composer and MVC architecture.

## Launch

-Clone repository to `www` folder inside root AMPPS directory\
[![1.png](https://i.postimg.cc/5Nw1Xz4d/1.png)](https://postimg.cc/1f5bTfVJ)\
\
-Create `sprint3` database on MySQL Workbench\
[![3.png](https://i.postimg.cc/6pF1NjZd/3.png)](https://postimg.cc/sM9JYJwX)
\
-Install composer if you haven't done that already:
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === '756890a4488ce9024fc62c56153228907f1545c228516cbf63f885e036d37e9a59d27d63f46af1d4d07ee0f76181c7d3') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```
\
-Run these commands in `sprint3` folder directory on terminal:
```
php composer.phar install
vendor\bin\doctrine orm:schema-tool:update --force --dump-sql
php composer.phar dump-autoload
```
\
-Enter this url to browser:\
[![2.png](https://i.postimg.cc/gj6WGXJJ/2.png)](https://postimg.cc/p5x7ZdKb)
