# 環境構築方法

### リポジトリから git clone してくる

```
git clone リポジトリURL
```

### ① 以下のコマンドを実行して、Dockerfile をビルドして docker image を作成する

```
docker compose build
```

### ② 以下のコマンドを実行して、作成した docker image から web コンテナを起動してコンテナ内に入り、開発用の db をセットアップする

```
docker compose run --rm web bin/setup
```

### ③ 以下のコマンドを実行して、web と db のコンテナを起動する

```
docker compose up
```

### ④ 以下の開発用アプリケーションの URL を web ブラウザで入力する

```
http://localhost:3000
```
