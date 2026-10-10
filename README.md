# qramo.github.io

[qramo.github.io](https://qramo.github.io) のソースです。[Astro](https://astro.build) で構築し、GitHub Actions で GitHub Pages に自動デプロイしています。

## 開発

```bash
npm install
npm run dev      # http://localhost:4321 で開発サーバーを起動
npm run build    # dist/ に静的サイトを出力
npm run preview  # ビルド結果をローカルでプレビュー
```

## 構成

- `src/pages/` — ページ（`index.astro` がトップページ、`works/` が作品一覧・詳細）
- `src/content/works/` — Works のコンテンツ（Markdown）
- `src/layouts/` — 共通レイアウト

`main` ブランチに push すると、`.github/workflows/deploy.yml` が自動でビルド・デプロイします。
