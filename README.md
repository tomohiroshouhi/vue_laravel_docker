## 環境情報
- php 8系
- Laravel8 そのうちLTSの９にしたい
- Vue 2.6.14
- Mysql 8.0
- Docker version 20.10.10, build b485636
- Docker Compose version v2.1.1

## 作業済み手順
### Docker関連
- 各コンテナのDockerfileを作成
- Docker-composeファイルを記述

### その他実行コマンド
- 以下のコマンドappコンテナに入る

```sh
$ docker-compose build
$ docker-compose up -d
$ docker-compose exec app bash
```

- コンテナの操作

```bash
# composer create-project --prefer-dist "laravel/laravel=8.*" .
# npm -v
# npm install -D vue-template-compiler
```

## 起動時のコマンド

```sh
$ docker-compose up -d
```

## 終了時のコマンド

```sh
$ docker-compose down
```

### 設定ファイル作成

docker-composeと同じ階層に以下の内容の.env作ってくれ！！

```text
WEB_PORT=80
DB_PORT=3306

DB_NAME=laravel
DB_USER=user
DB_PASSWORD=root
DB_ROOT_PASSWORD=password
```