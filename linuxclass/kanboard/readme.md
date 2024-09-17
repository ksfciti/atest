# step by step
``` bash
vagrant ssh  
```
## install apache
``` bash
sudo dnf search httpd
sudo dnf install -y httpd
```

## install php 
``` bash 
sudo dnf install -y php php-mysqlnd
```
### install php modules 
``` bash 
sudo dnf install -y php-gd php-mbstring php-json php-xml
```
### start and enable web server
``` bash 
sudo systemctl start httpd
sudo systemctl enable httpd
```

## install mariadb 
``` bash
sudo dnf install -y mariadb-server
sudo systemctl start mariadb
sudo systemctl enable mariadb 
```

### secure mariadb
``` bash 
sudo mysql_secure_installation
mysqladmin -u root -p create kanboard
mysql -u root -p
```
press ENTER 
``` bash
curl -LO http://mirror.linuxtrainingacademy.com/kanboard/kanboard-v1.2.15.zip 
unzip kanboard-v1.2.15.zip
sudo mv kanboard-1.2.15/* /var/www/html
ls -l /var/www/html
sudo nano /var/www/html/config.php
```
