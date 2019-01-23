
# Docker / PHP / Nginx / MongoDB / MySQL
This is a docker-compose file for start nginx ,php-fpm ,mongoDB and mysql.


## How to use
You need to have a Docker (docker >= 17.12.0+) setup (See Testing for a local setup) and install [docker-compose](https://docs.docker.com/compose/install/)


### Quick Start
Run these commands:
```
$ git clone https://github.com/saderi/L3
$ cd L3
$ docker-compose up -d
```  
Copy your project file inside in html folder.

## Access to phpMyAdmin: 
* **URL:** `http://localhost:8086`
* **Server:** mysql_server
* **Username:** root
* **Password:** root (as a default)

## Environments
You can config the following environment variables for create and start containers. Stack works correctly with the default value, but it's better if you config them.

* `YOUR_PROJECT_PATH`, the default value is  `./html`
* `MARIADB_VERSION`, the default value is `10.2.21`
* `MYSQL_DATA_PATH`, the default value is `mysql` # use volume by default, you can change it if you want use specify path.
* `WEBROOT`, the default value is `/var/www/html`
* `MYSQL_ROOT_PASSWORD`, the default value is `root`
* `PHPMYADMIN_ACCESS_PORT`, the default value is `8086`
* `MONGOBD_DATA_PATH`, the default value is `mongodb` # use volume by default, you can change it if you want use specify path.
* `MONGO_VERSION`, the default value is `4.1.6`
* `MONGO_INITDB_ROOT_USERNAME`, the default value is `admin`
* `MONGO_INITDB_ROOT_PASSWORD`, the default value is `admin123`
* `NETWORK_NAME`, the default value is `my-stack-network`


**Attention: Don't use this repository on production :D**