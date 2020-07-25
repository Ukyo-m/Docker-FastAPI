# Docker-FastAPI

FastAPIのプロジェクトを構築するためのリポジトリです。

## 手順

1. イメージの作成  
   `docker-compose build`
2. コンテナの立ち上げ
   `docker-compose up -d`

## フォルダ構成

```
Docker-FastAPI
┃
┣━api
┃  ┃
┃  ┣━src // ソースファイル
┃  ┃
┃  ┣━Dockerfile
┃  ┃
┃  ┗━requirements.txt
┃
┃
┗━mysql
┃   ┃
┃   ┣━conf.d
┃   ┃   ┗━my.cnf // 設定ファイル
┃   ┃
┃   ┣━initdb.d // 初期ファイル
┃   ┃           // コンテナ立ち上げ時にこのフォルダを読み込んでDBを作成してくれる
┃   ┃
┃   ┣━logs // ログファイル
┃   ┃
┃   ┗━Dockerfile
┃
┃
┗━docker-compose.yml 
```
