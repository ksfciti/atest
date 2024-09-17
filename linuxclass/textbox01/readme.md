# installing apache 
``` bash
dnf search apache server
dnf info httpd
sudo dnf install httpd

sudo systemctl start httpd
sudo systemctl enable httpd
sudo systemctl enable --now httpd
```

# install maria db 
``` bash 

dnf search mariadb 
dnf info mariadb-server
sudo dnf install mariadb-server
# sudo -s; whoami 
sudo systemctl start mariadb.service 
sudo systemctl enable mariadb.service

systemctl } grep mariadb

sudo systemctl status mariadb-service
sudo systemctl is-active mariadb-service
mysqlshow 
top
```
### mysql_secure_insstallation 
``` bash 
sudo mysqladmin -u root -p<haslo> create newdb 
```
# install php 
``` bash 
dnf search php
sudo dnf install -y php php-mysqlnd
sudo systemctl reload httpd 
sudo systemctl restart httpd 

systemctl status httpd

```

