# nginx_php-fpm_maria_redis
nginx, php-fpm, mariadb, redis

### HOW TO USE
#### Install Docker-Compose
```
curl -L https://github.com/docker/compose/releases/download/1.14.0-rc2/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```

#### 1) Clone project
```
git clone https://github.com/devjiro76/nginx_php-fpm_maria_redis
cd nginx_php-fpm_maria_redis
```

#### 2) Make this project your owns (If you want)
```
rm -rf .git
```

#### 3) test with phpinfo
Create a new file as "web/phpinfo.php"
```
<?php
phpinfo();
```

#### 4) Set your DB Root Password
```
vi docker-compose.yml
```
and change the '<YOUR_PASSWD>' to what you want

#### 5) RUN
```
docker-compose up -d
```

#### 6) Check phpinfo
Open `http://localhost/phpinfo.php` on your browser
