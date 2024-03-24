# A first-level headingprometheuse_mysql_grafana
## Установка прокекта
> git clone  https://github.com/AleksandrSRS/prometheuse_mysql_grafana.git
cd prometheuse_mysql_grafana
cat <<EOF >>brightup.sh
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
## A second-level heading
### A third-level heading
