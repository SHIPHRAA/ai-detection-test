# Platform Template

[![Release Production](https://github.com/dtgrid/dg-platform-template/actions/workflows/release-prod.yaml/badge.svg)](https://github.com/dtgrid/dg-platform-template/actions/workflows/release-prod.yaml)

## ディレクトリ構成

```bash
|-- backend
|-- backend-ml
|-- frontend
|-- docker-compose.local.yml
|-- docker-compose.local.gpu.yml
|-- Makefile
`-- README.md
```

## 開発環境構築

### 概要

下の手順に従ってコマンドを流して全てのコンポーネントの環境を構築することができます。詳細に関しては各コンポーネント下の README.md を参照ください。

コンポーネントは以下のように別れています。

- backend...バックエンドコンポーネント
- backend-ml...機械学習周りのバックエンドコンポーネント群
- frontend...フロントエンドコンポーネント

### 手順

#### FE

https://github.com/dtgrid/dg-platform-template/tree/main/frontend の README.md を参照。

#### BE

https://github.com/dtgrid/dg-platform-template/tree/main/backend の README.md を参照。

### 2-3. DB データ削除

DB 不整合状態などが起きた場合は以下のコマンドで DB を全削除することができます。

```sh
$ make db-delete-data
```

## 3. 本番リリース

タグをつけることで frontend/backend/ml-backend がリリースされます。

タグ名は「YYYY.MM.DD-index 番号」としてください。
