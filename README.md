# docker-php-nginx-mysql

Using docker-compose to run PHP-FPM, MYSQL, PMA and NginX.

## Usage:
1. `git clone https://github.com/VirgoSep72016/docker-php-nginx-mysql.git`
1. Add hosts: `127.0.0.1 default_server php_server`
1. Run docker-compose: `env UID=$(id -u) GID=999 docker-compose up`

### Set Nginx:

You can set custom nginx.conf at: `./docker_config/nginx/conf.d/project_conf/CustomNginX.conf`

### Create Project:

You can create own project at: `./project/YourProject`

### Custom docker-compose

You can change `nginx` or `project` volumes at: `./docker-compose.yml`

## Sites:

* pma: [http://127.0.0.1:8081/](http://127.0.0.1:8081/)
* php_server: [http://php_server:8080/](http://php_server:8080/)
* default_server: [http://default_server:8080/](http://default_server:8080/)
