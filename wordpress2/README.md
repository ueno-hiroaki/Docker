### 起動の仕方
```
docker compose up -d
```
<font color="red">※compose.yamlのディレクトリで実行すること！</font>
| 環境変数              | 意味                                                       | 
| :-------------------- | ---------------------------------------------------------- | 
| WORDPRESS_DB_HOST     | 接続先のコンテナ名。compose.yamlで定義した名前を設定する。 | 
| WORDPRESS_DB_NAME     | 接続先データベースのデータベース名                         | 
| WORDPRESS_DB_USER     | 接続先データベースのユーザー名                             | 
| WORDPRESS_DB_PASSWORD | 接続先データベースのパスワード                             | 

 

[DockerHub:wordpress](https://hub.docker.com/_/wordpress)

 
[WordPressへのアクセス](http://localhost:8080/)

ホストOSのhtmlフォルダをwordpressコンテナの/var/www/htmlフォルダをバインドマウント