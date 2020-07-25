FROM python:3.7

RUN apt update

WORKDIR /usr/src/server
ADD requirements.txt .
# requirements.txtにリストされたパッケージをインストールする
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# コンテナ起動後、FastAPIを実行し8080ポートで待機
# CMD ["uvicorn", "main:app", "--reload", "--host", "0.0.0.0", "--port", "8080"]