# Laravel Docker Compose Setup

## What it provides
- Nginx
- PHP 7.3 (PHP-FPM)
- Redis
- MariaDB
- Beanstalkd

##### PHP Extensions
- xDebug (if built in dev mode)
- gd
- bcmath
- iconv
- intl
- mbstring
- mysqli
- opcache (if build in prod)
- pdo
- pdo_mysql
- zip

## Requirements
- Docker
- Docker compose

## Installation
First copy the ```.env.dist``` file to ```.env``` and enter the default details.
Depending on the environment, you'll get a different build of PHP. In development, you'll get PHP-FPM 7.3 with
xDebug installed. In production, you won't have xDebug installed.

Install in dev:
```bash
$ docker-compose up -d
```

*The ```-d``` flag will tell docker to start the containers in the background*

## Suggestions
If you have any suggestions and/or improvements please open an issue on Github.
