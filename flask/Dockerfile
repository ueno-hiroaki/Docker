FROM python:3.10
#イメージの指定
WORKDIR /usr/src/app
#作業ディレクトリの指定
RUN pip install flask==2.1.0
#RUNなのでイメージのビルド時にコマンドを実行
CMD ["flask","run","--host=0.0.0.0"]
#CMDなのでコンテナの起動時にコマンドを実行
