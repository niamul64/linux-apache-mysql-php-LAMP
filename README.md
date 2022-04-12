## uninstall linux-apache-mysql-php-LAMP
https://gist.github.com/UbuntuEvangelist/9d115b4ca95c330ef6d2dd42f6c133c9

## if ubuntu settings file problem: sudo apt install gnome-control-center

## install linux-apache-mysql-php-LAMP
## follow:
https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-20-04


Or, https://www.youtube.com/watch?v=vazRx1Ei8VA
### don't install php my admin

<hr> 
if don't want to use nano
give edit permission to a directory: sudo chmod -R 777 /var/www
here '/var/www' directory name
<hr>
ububtu mysql database root pass: june221996

<hr>

## reload apache server: sudo systemctl reload apache2

## If any problem to activate the apache then
## active server
$ sudo a2ensite smbFileSystem.conf
$
##  disable runing server:
$ sudo a2dissite smbFileSystem.conf
$
### restart apache2 : sudo service apache2 restart
## run php code vertual host: https://www.youtube.com/watch?v=Vd2aLTZDLQg





