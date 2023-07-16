## ファイル・ディレクトリ構成

docker
├─nginx
│ ├─Dockerfile
│ └─default.conf
└─php
  ├─src
  │ └─.gitkeep
  ├─Dockerfile
  └─php.ini
.gitignore
README.md
compose.yaml

## 環境構築
```bash
$ docker-compose up -d
$ docker-compose exec app bash

# appコンテナ内
# appの部分はプロジェクト名なので適宜変更する
$ composer create-project "laravel/laravel=10.*" laravel10 --prefer-dist
```

## URL
http://localhost/