### 起動の仕方
コンテナの作成と実行
<font color="red">compose.yamlを配置した階層で実行する</font>
```
docker compose up -d
```
実行中のコンテナを一覧表示 全部表示させるなら -a をつける
```
docker container ls
```
コンテナを停止
```
docker compose stop
```
コンテナを起動
```
docker compose start
```