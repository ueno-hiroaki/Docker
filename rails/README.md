**1. コンテナ作成の準備**
<font color="red">railsプロジェクトの作成が必要！</font>
```shell
docker compose run --rm web rails new . --force --no-deps --database=mysql
```

**2. イメージを再びビルド**
```
docker compose build
```

**3. database.ymlの編集**
Railsの接続先をMariaDBコンテナにする
config/database.yml(抜粋)
```yaml
default: &default
  adapter: mysql2
  encoding: utf8mb4
  pool: <%= ENV.fetch("RAILS_MAX_THREADS") { 5 } %>
  username: root
  password: <%= ENV.fetch("DATABASE_PASSWORD") %>
  host: db
  port: 3306
```
**4. コンテナの作成**
```
docker compose up -d
```
**5. データベースの作成**
Railsを起動するには事前にデータベースを作成する必要がある
```
docker compose exec web rake db:create
```
http://localhost:3000
へアクセス