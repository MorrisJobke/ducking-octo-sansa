```
pacman -S php php-fpm php-gd php-intl php-mcrypt php-sqlite apache
systemctl enable httpd
systemctl enable php-fpm
sudo mkdir /srv/http/owncloud
sudo chown mjob:users /srv/http/owncloud
git clone https://github.com/owncloud/core /srv/http/owncloud
cd /srv/http/owncloud
git submodule update --init
```
