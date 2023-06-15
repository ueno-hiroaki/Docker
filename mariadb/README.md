### MARIADBイメージの主な環境変数
| 環境変数         | 意味                       |
| :--------------: | :------------------------: | 
| MARIADB_PASSWORD | ルートユーザーのパスワード | 
| MARIADB_DATABASE | データベース名             | 
| MARIADB_USER     | データベースのユーザー名   | 
| MARIADB_PASSWORD | データベースのパスワード   | 

[DockerHub:mariadb](https://hub.docker.com/_/mariadb)

### コンテナの中に入る方法
```
docker compose exec db /bin/bash
```
#### データベースに入る
```
mariadb -u testuser -D testdb -p
```
#### mariaDBのCLIを終了する
```
\q
から
exit
```
