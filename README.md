# Uninstalling-Pterodactyl

# Uninstall Panel

## Panel files
```bash
sudo rm -rf /var/www/pterodactyl
```
## If using nginx
```bash
sudo unlink /etc/nginx/sites-enabled/pterodactyl.conf
```
## If using apache
```bash
sudo unlink /etc/apache2/sites-enabled/pterodactyl.conf
```
_________________________________________________________________
# Uninstall Wings

## Stop the Wings
```bash
sudo systemctl stop wings
```
## Game server files and backups
```bash
sudo rm -rf /var/lib/pterodactyl
```
## Wings config
```bash
sudo rm -rf /etc/pterodactyl
```
## Wings binary
```bash
sudo rm /usr/local/bin/wings
```
## Wings daemon file
```bash
sudo rm /etc/systemd/system/wings.service
```
_______________________________________________________________________________________

# Uninstall Web Server (optional)
## NGINX

## If using debian/ubuntu
```bash
sudo systemctl stop nginx
```
```bash
sudo apt purge nginx nginx-common
```
```bash
sudo apt autoremove # remove any leftover dependencies
```
## If using CentOS
```bash
sudo service nginx stop
```
```bash
sudo yum remove nginx
```

## Apache

## If using Ubuntu/Debian
```bash
sudo systemctl stop apache2
```
```bash
sudo apt purge apache2
```
```bash
sudo apt autoremove
```

## If using CentOS
```bash
sudo service apache2 stop
```
```bash
sudo yum erase httpd httpd-tools apr apr-util
```
