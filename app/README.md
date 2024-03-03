# 書籍おすすめプログラム

## 必要環境

- docker version 20.10.x 以上

## セットアップ方法

```console
$ docker compose build
$ docker compose up -d
```

## 実行方法

例: 入出力データディレクトリを `data/` とする場合

- `data/` に `yomilog.csv` を配置

```console
$ docker compose exec app python recommend_books.py susumuis 5000 -i data -o data -l DEBUG
```

- `data/` に `result-susumuis-5000.csv` などの結果が出力される
