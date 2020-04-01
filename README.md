# nginx_php_docker
nginx php docker compose
docker 启动 nginx + php-fpm + redis + mysql

https://docs.docker.com/compose

安装 docker compose

sudo curl -L https://get.daocloud.io/docker/compose/releases/download/1.25.0/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose

systemctl start docker
systemctl restart docker
systemctl status docker
docker info

cd compose.yaml 所在目录 ,docker-compose up -d / docker-compose down

