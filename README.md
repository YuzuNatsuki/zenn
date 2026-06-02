# Zenn コンテンツ

[Zenn](https://zenn.dev) の記事をGitHubで管理するリポジトリです。

## フォルダ構成

```
.
├── articles/   # 記事 (.md)
└── .github/
    └── workflows/
        └── publish.yml  # GitHub Actions（自動チェック）
```

## 記事の作成

### Zenn CLI を使う場合（推奨）

```bash
npm install -g zenn-cli
npx zenn new:article
```

### 手動作成

`articles/` 以下に `slug.md` を作成し、以下のfrontmatterを記載：

```yaml
---
title: ""
emoji: "✨"
type: "tech"  # tech or idea
topics: []
published: false
---
```

## GitHub連携の設定

1. このフォルダを `git init` してGitHubにpush
2. [Zenn](https://zenn.dev/dashboard/deploys) でリポジトリを連携

詳細: https://zenn.dev/zenn/articles/connect-to-github
