_ _ _ ___     ___  ____ ____ _  _ ____ ____ 
| | | |__] __ |  \ |  | |    |_/  |___ |__/ 
|_|_| |       |__/ |__| |___ | \_ |___ |  \


Use this to run WordPress local development environment using Docker-Compose.

Step 1. After cloning this repo., goto the directory.
Step 2. Make necessary changes in docker-compose.yml according to convenience like ports to be exposed, directories etc. and finally hit sudo docker-compose up -d
Step 3. This will start 3 containers one official WordPress with inbuilt webserver and others for MariaDB and PhpMyAdmin
Verify if all 3 containers are up and running with sudo docker ps
Step 4. Your WordPress content will be in htdocs folder and that of DB will be in mysql folder.
Step 5: Install & Access WordPress at http://127.0.0.1:8080 and PhpMyAdmin at http://127.0.0.1:8181

default credentials:

MYSQL_USERNAME: root
MYSQL_ROOT_PASSWORD: pass@123
PMA_HOST: wordpress_db
WORDPRESS_DB_PASSWORD: pass@123
WORDPRESS_DB_NAME: wpdb
WORDPRESS_TABLE_PREFIX: wp_
WORDPRESS_DB_HOST: wordpress_db
