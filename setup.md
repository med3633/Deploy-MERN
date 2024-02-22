# open firewall or show command in ufw
```bash
ufw --help
```
# show app
```bash
ufw app list
```
```bash
git clone https://github.com/youssef-of-web/crud-users-tutorial.git
```
# use pm2 => demarre server
```bash
npm i -g pm2
```
```bash
pm2 stat "npm un start"
```
## build react app se form index et dossier static
```bash
npm run build
```
```bash
cd build
```
## copir folder build sous /var/www/ de nginx
```bash
cp -R .. ..
```
## install nginx
```bash
apt get nginx
```
## lien symbolique available and enabled
```bash
nano test.com
```
### write nginx config
```bash
server {
listen 80;
server_name www.test.com;
 location / {
# win mawjoud il build
 root /data/www/build/;
# wil index
index index.htm index.html;
}
#request
location /api {
# connect client t server
proxy_pass http://@ip:port/api ;
}
}
```
# check nginx
```bash
nginx -t
```
## do lien sybolique and restart nginx
```bash
cd etc/nginx/sites-available
ln -s /etc/nginx/sites-available/test.com /etc/nginx/sites-enabled/test.com
```
## certificat
```bash
certbot --nginx
```


