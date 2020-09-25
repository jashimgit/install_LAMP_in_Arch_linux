#How to install Apache, PHP, mysql, phpmyadmin in Arch linux

https://ostechnix.com/install-apache-mariadb-php-lamp-stack-on-arch-linux-2016/


1. Update your Arch system { type this command in terminal }
pacman -Syu
2. Install Apache
pacman -S apache
Edit /etc/httpd/conf/httpd.conf file

nano /etc/httpd/conf/httpd.conf
Search and comment out the following line if it is not already:
[...]
#LoadModule unique_id_module modules/mod_unique_id.so
[...]
save file and run the following command
systemctl enable httpd
systemctl restart httpd
