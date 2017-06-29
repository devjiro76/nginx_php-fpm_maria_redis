# nginx_php-fpm_maria_redis
nginx, php-fpm, mariadb, redis

### HOW TO USE
#### Install Docker-Compose
```
curl -L https://github.com/docker/compose/releases/download/1.14.0-rc2/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```

#### Clone project
```
git clone https://github.com/devjiro76/nginx_php-fpm_maria_redis
cd nginx_php-fpm_maria_redis
```

#### Make the project as yours
```
rm -rf .git
```

#### test with phpinfo
Create a new file as "web/phpinfo.php"
```
<?php
phpinfo();
```

#### RUN
```
docker-compose up -d
```

#### Check phpinfo
Open `http://localhost/phpinfo.php` on your browser
