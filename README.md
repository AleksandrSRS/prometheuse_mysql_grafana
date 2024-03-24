# A first-level headingprometheuse_mysql_grafana
## Подготовка

```
Заполнить файл hosts в зависимости от вашей ОС
XXX.XXX.XXX.XXX		wp.local #URL - Wordpress -> /conf.d/nginx.conf
XXX.XXX.XXX.XXX		metrics.local #URL - Grafana -> /conf.d/nginx.conf
```

## Установка прокекта
```
git clone  https://github.com/AleksandrSRS/prometheuse_mysql_grafana.git
cd prometheuse_mysql_grafana
```
Внесите изменеие
```
cat <<EOF >>.env
#!/bin/sh
MYSQL_DATABASE=dbwordpress
MYSQL_USER=wpuser
MYSQL_PASSWORD=wppassword
MYSQL_ROOT_PASSWORD=wprootpassword

WORDPRESS_DB_HOST=db
WORDPRESS_DB_NAME=dbwordpress
WORDPRESS_DB_USER=wpuser
WORDPRESS_DB_PASSWORD=wppassword
EOF
```
## Запуск
```
docker compose up -d
```
## Инициализация DB Wordpress
http://wp.local
### Gragana URL
http://metrics.local
