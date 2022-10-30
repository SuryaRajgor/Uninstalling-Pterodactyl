# Uninstalling-Pterodactyl

# Uninstall Panel


# Panel files
```bash
sudo rm -rf /var/www/pterodactyl
```
# If using nginx
```bash
sudo unlink /etc/nginx/sites-enabled/pterodactyl.conf
```
# If using apache
```bash
sudo unlink /etc/apache2/sites-enabled/pterodactyl.conf
```
