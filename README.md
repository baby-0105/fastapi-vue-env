# セットアップ

```
$ cp .env.template .env
$ docker network create fastapi_network

.envの mysql用の定数を各々で設定

$ docker-compose up -d
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
https://zenn.dev/yusugomori/articles/a3d5dc8baf9e386a58e5

https://github.com/testdrivenio/fastapi-vue
