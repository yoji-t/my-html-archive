# My HTML Archive - GitHub Pages

競馬回顧や考察などの単体HTMLをどんどん溜めていくための、GitHub Pages用テンプレートです。

## 特徴
- Jekyll不要、ビルド不要。静的ファイルだけ。
- `articles/` にHTMLを置く + `data.json` に1行追記で一覧に自動表示
- 検索・タグフィルタ付きのトップページ
- レスポンシブ、おしゃれなカードUI

## フォルダ構成
```
/
├─ index.html      # 一覧ページ
├─ data.json       # 記事メタデータ
├─ assets/style.css
└─ articles/
   └─ hanshin-daishoten-1996.html  # サンプル
```

## 使い方
1. このリポジトリをGitHubにPush
   ```
   git init
   git add .
   git commit -m "initial"
   git remote add origin https://github.com/USERNAME/REPO.git
   git push -u origin main
   ```
2. GitHub > Settings > Pages > Build and deployment: `Deploy from a branch` > `main / root` を選択
3. 数分で公開されます

## 新しいHTMLを追加
1. `articles/new-article.html` を作成
2. `data.json` に追記:
```json
{
  "id": "new-article",
  "title": "タイトル",
  "file": "new-article.html",
  "date": "2026-10-03",
  "tags": ["競馬"],
  "summary": "要約"
}
```

## カスタマイズ
- サイトタイトルは `index.html` の `<h1>` を変更
- 色は `assets/style.css` の `:root` で変更

MIT License
