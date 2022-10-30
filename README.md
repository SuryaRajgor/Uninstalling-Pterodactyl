# Uninstalling-Pterodactyl

# Uninstall Panel

```
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
```
```
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
```
