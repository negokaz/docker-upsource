[Upsource](https://www.jetbrains.com/upsource/) をインストールした Docker image です

使い方
------

~~~
docker run --name upsource \
  -d \
  -p {PORT}:8080 \
  -v {CONF_DIR}:/opt/Upsource/conf \
  -v {DATA_DIR}:/opt/Upsource/data \
  -v {LOGS_DIR}:/opt/Upsource/logs \
  -v {BACKUP_DIR}:/opt/Upsource/backups \
  negokaz/upsource
~~~

* {PORT} - Upsource のサービスにアクセスするためのポート番号

ブラウザで`http://{DOCKER_HOST}:{PORT}`へアクセスすると Upsource のページが表示されます。

* {DOCKER_HOST} - Docker のホスト名もしくはIPアドレス
