# Uninstalling-Pterodactyl

# Uninstall Panel

```# Panel files
sudo rm -rf /var/www/pterodactyl

# Pteroq queue worker
sudo rm /etc/systemd/system/pteroq.service

# If using nginx
sudo unlink /etc/nginx/sites-enabled/pterodactyl.conf

# If using apache
sudo unlink /etc/apache2/sites-enabled/pterodactyl.conf```
