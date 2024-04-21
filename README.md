# 個人開発環境用リポジトリ
node.jsベースのアプリケーション & DB（Mysql） のコンテナを起動するために作ったリポジトリ
 - フロントエンド用コンテナ：app_frontend
 - バックエンド用のコンテナ：app_backend
 - DB用のコンテナ：db_container（db）

## 利用ポート
フロントエンド: 3000
バックエンド: 8000

## コンテナ起動方法
`docker-compose build`  
`docker-compose up -d`
