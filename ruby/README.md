### 起動の仕方
コンテナの作成と実行
<font color="red">compose.yamlを配置した階層で実行する</font>
```
docker compose up -d
```

### test.rbの実行方法
```
docker compose exec ruby ruby /src/test.rb
```