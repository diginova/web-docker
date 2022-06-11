# Clone
git clone https://github.com/diginova/web-docker.git
# Run
docker-compose up -d

(Visit: http://127.0.0.1)

# Run Bash
docker-compose run php bash

# Stop
docker-compose down

# Add VirtualHost
* Create new directory for new virtual-host in app directory.
* Copy config file (sites-enabled/default.conf) with new name for new virtual-host in same directory. Configure path and domain.
* Add new domain record to /etc/hosts (like: 127.0.0.1    default)
* Restart docker-compose container (down and up)

# PhpMyAdmin
* Visit http://127.0.0.1:8080 (server:db / username:root / password:root)
