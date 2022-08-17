* Docker 立ち上げ

```sh
$ docker-compose up -d
```

* seeding
  * サンプルデータの作成

```sh
$ docker-compose exec back bash
# cd /usr/src/app/db
# python seed.py
```
