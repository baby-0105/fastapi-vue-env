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

## local host

```
http://localhost:8888/docs # Open API
http://localhost:8080
```

# 参考
https://zenn.dev/yusugomori/articles/a3d5dc8baf9e386a58e5#%E3%83%9E%E3%82%A4%E3%82%B0%E3%83%AC%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%E8%A8%AD%E5%AE%9A

https://github.com/testdrivenio/fastapi-vue
