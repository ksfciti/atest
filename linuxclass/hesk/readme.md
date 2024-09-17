``` bash
sudo dnf install -y httpd
sudo dnf install -y php php-mysqlnd
sudo systemctl start httpd
sudo systemctl enable httpd
sudo dnf install -y mariadb-server
sudo systemctl start mariadb
sudo systemctl enable mariadb 
sudo mysql_secure_installation
```
## create database hesk 
``` bash 
mysqladmin -u root -p create hesk
mysql -u root -p 
GRANT ALL on hesk.* to hesk@localhost identified by 'hesk123';
FLUSH PRIVILEGES;
exit 
mysqlshow -u root -p 

```

http://mirror.linuxtrainingacademy.com/hesk/
curl -LO http://mirror.linuxtrainingacademy.com/hesk/hesk343.zip 

pwd

cd /var/www/html/
sudo unzip /home/vagrant/hesk343.zip 
sudo chown apache hesk_settings.inc.php 
sudo chown apache attachments
sudo chown apache cache
sudo chown apache language/

goto 

sudo dnf install -y php-json

http://192.168.56.4/install

