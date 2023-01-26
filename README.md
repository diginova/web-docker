# Clone
```sh
git clone https://github.com/diginova/web-docker.git
```

# Run
### If you are installing for Yii2:
```sh
docker-compose -p web-docker-yii2 -f yii2.yml up -d
```
### If you are installing for Laravel:
```
docker-compose -p web-docker-laravel -f laravel.yml up -d
```

> Visit: http://127.0.0.1

# Run Bash
```sh
docker-compose run php bash
```

# Stop
```sh
docker-compose -p web-docker-yii2 -f yii2.yml down
```
or
```sh
docker-compose -p web-docker-laravel -f laravel.yml down
```

# Add VirtualHost
* Create new directory for new virtual-host in app directory.
* Copy config file (sites-enabled/default.conf) with new name for new virtual-host in same directory. Configure path and domain.
* Add new domain record to /etc/hosts (like: 127.0.0.1    default)
* Restart docker-compose container (down and up)

# PhpMyAdmin
* Visit http://127.0.0.1:8080 (server:db / username:root / password:root)
