FROM python:3.10
WORKDIR /code
#addでrequirements.txtを追加しておくことでpipコマンド実行時にrequirements.txtを読み込む installするものをrequirements.txtに書く
ADD requirements.txt /code/
#requirements.txtにまとめておき、コマンドで実行すると複数ライブラリを一括でインストールできる これはpipの機能
RUN pip install -r requirements.txt
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
#dockerfileはイメージからイメージを作る
