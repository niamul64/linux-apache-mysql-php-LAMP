## uninstall linux-apache-mysql-php-LAMP
https://gist.github.com/UbuntuEvangelist/9d115b4ca95c330ef6d2dd42f6c133c9

## if ubuntu settings file problem: sudo apt install gnome-control-center

## install linux-apache-mysql-php-LAMP
## follow:
https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-20-04

Or, https://www.youtube.com/watch?v=46_hyK-uBrQ&t=8s
### keep security lite install php my admin

<hr> 
if don't want to use nano
give edit permission to a directory: sudo chmod -R 777 /var/www
here '/var/www' directory name
<hr>

## reload apache server: sudo systemctl reload apache2
### restart apache2 : sudo service apache2 restart
<hr>

# Now wirtual host:
### run php code vertual host: https://www.youtube.com/watch?v=Vd2aLTZDLQg

## if project file name is: smbFileSystem
This project file is need to be inside computer/var/www/

## default and vertual host are at--> /etc/apache2/sites-available/

```
inside: sites/apache2/sites-available/smbFileSystem.conf
<VirtualHost *:80>
    ServerName smbFileSystem.com
    ServerAlias www.smbFileSystem.com 
    ServerAdmin smbFileSystem.com
    DocumentRoot /var/www/smbFileSystem
    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
see other files inside: sites/apache2/sites-available/
https://github.com/niamul64/PHP-crud-smb-file-share
```
## If any problem to activate the apache then
## active the virtualserver:
$ sudo a2ensite smbFileSystem.conf
$ sudo service apache2 restart

### disable the default one
$ sudo a2dissite 000-default.conf
$ sudo service apache2 restart
##  disable runing server:
$ sudo a2dissite smbFileSystem.conf
$ sudo service apache2 restart







