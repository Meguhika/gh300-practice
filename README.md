# GH-300 Practice Repository

GitHub Actions認定試験(GH-300)の学習用リポジトリです。

## 演習内容

### 1. ワークフロー構文基礎：`/` と `@` の使い方
- `/`: ワークフロー内でのアクション参照のパス区切り
- `@`: アクションのバージョン指定子

**学習ポイント**
- `owner/repo@ref` 形式でのアクション指定
- `ref` の種類（ブランチ、タグ、コミットSHA）
- 相対パスでのローカルアクション参照

### 2. コンテンツ除外管理
- `.gitignore`: Gitが追跡しないファイルを指定
- `.github/workflows/.gitignore`: ワークフロー関連のファイル除外
- 環境変数でのシークレット管理

**学習ポイント**
- シークレット値の外部ファイル化を避ける
- ビルド成果物の除外設定
- ログファイルの管理

## 演習ディレクトリ構成

```
.
├── .github/
│   ├── workflows/
│   │   ├── 01-basic-syntax.yml      # 演習1: 基本構文
│   │   └── 02-content-exclusion.yml # 演習2: コンテンツ除外
│   └── actions/
│       └── custom-action/           # カスタムアクション例
├── .gitignore
├── README.md
└── exercises/
    ├── 01-syntax/
    └── 02-exclusion/
```

## 進め方

1. `.github/workflows/01-basic-syntax.yml` を確認
2. `@` と `/` の使用例を学ぶ
3. `.github/workflows/02-content-exclusion.yml` を確認
4. `.gitignore` と除外ルールを実装
5. 実際に実行して動作確認

---

**作成日**: 2026-10-11  
**目的**: GH-300認定資格取得のための実践演習
