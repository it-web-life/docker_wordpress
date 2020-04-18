# docker_wordpress
Build a WordPress environment with Docker

【初心者向け】DockerでWordPressを動かす方法を解説
https://it-web-life.com/docker-wordpress/

## usage
本リポジトリを`git clone`します。

### Dockerの起動
cloneしたディレクトリに移動して、`docker-compose up`コマンドを実行します。
`$ docker-compose up -d`

- WordPressが`localhost:8000`で起動します。
- phpMyAdminが`localhost:8080`で起動します。

### Dockerの起動状況の確認
- `$ docker ps -a`
  Dockerのコンテナの状況を確認することができます。

- `$ docker volume ls`
  Dockerのvolumeを確認できます。

### Dockerの停止方法
- `$ docker-compose stop`
  一時的に停止できます。

### Dockerを再度起動させる方法
- `$ docker-compose restart`
  一時的に停止したコンテナを再起動できます。

### Dockerのコンテナを削除する方法
- `$ docker-compose down`
  コンテナを削除できます。


### Dockerのコンテナと設定もすべて削除する方法
- `$ docker-compose down --volumes`
  Dockerのコンテナだけでなく、WordPressで設定したデータなど含めて、volumesのデータも消します。
  手動でディレクトリ内の「html」「phpmyadmin」ディレクトリも削除して下さい。
