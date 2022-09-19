# セットアップ

## Docker 立ち上げ

```sh
$ docker-compose up -d
```

## .env

```
cp .env.template .env
```

.envの編集

```
COMPOSE_PROJECT_NAME=fastapi_vue_env

MYSQL_USER=[各々で記載]
MYSQL_PASSWORD=[各々で記載]
MYSQL_ROOT_PASSWORD=[各々で記載]
MYSQL_HOST=[各々で記載]
MYSQL_DATABASE=[各々で記載]

PYTHONPATH=/usr/src/app/backend
```

## seeding
サンプルデータ作成

```sh
$ docker-compose exec back bash
# cd /usr/src/app/db
# python seed.py
```
