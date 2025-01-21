# Presentations

このリポジトリは、[Marp](https://marp.app/)を使用してスライドを作成・管理するためのプロジェクトです。

## 🚀 特徴

- Markdownベースのスライド作成
- 一貫性のあるデザインルール
- バージョン管理可能なスライド

## 📦 必要条件

- Node.js (最新の安定版を推奨)
- VSCode + [Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)
- @marp-team/marp-cli (スライドのエクスポート用)

## 🛠 セットアップ

1. リポジトリのクローン:
```bash
git clone https://github.com/chocopie116/presentations.git
cd presentations
```

2. Marp CLIのインストール:
```bash
npm install -g @marp-team/marp-cli
```

3. VSCodeでプロジェクトを開く:
```bash
code .
```

4. Marp for VS Code拡張機能をインストール

## 🎯 スライドの出力

### PDFとして出力
```bash
marp 20241211_ragaiagent/スライド.md --pdf -o ~/Desktop/ragaiagent_presentation.pdf
```

### HTMLとして出力
```bash
marp 20241211_ragaiagent/スライド.md --html -o ~/Desktop/ragaiagent_presentation.html
```

### PowerPointとして出力
```bash
marp 20241211_ragaiagent/スライド.md --pptx -o ~/Desktop/ragaiagent_presentation.pptx
```

### プレゼンテーションモード（ライブプレビュー）
```bash
marp -s .
```

## 📝 スライド作成ルール

### 1. スライド構造

#### タイトルスライド（1枚目）
- `#` でタイトルを指定
- `##` でサブタイトルを指定
- 発表者名を含める
- 背景画像を設定（暗めの画像を推奨）

#### 基本スライド
- `#` でタイトルを指定
- 必要に応じて `##` でサブタイトルを使用
- h2（`##`）は1スライドに2回以上使用禁止
- h3の使用は禁止

### 2. デザイン規則

#### 背景画像の指定
- 全面背景: `![bg cover](path/to/image)`
- 右配置: `![bg right:40%](path/to/image)`
- 明るさ調整: `brightness:0.4` などで指定

#### テキストカラー
必要な場合はディレクティブを使用:
```markdown
<!-- _color: white -->
```

### 3. コンテンツ構成

1スライドあたり以下のいずれかのパターンに従う:
- 見出し + 3-5個の箇条書き
- 見出し + 1枚の大きな画像
- 見出し + 右側40-60%の画像 + 左側テキスト

## 📂 ディレクトリ構造

```
presentations/
├── README.md
└── {YYYYMMDD}_{プレゼン名}/
    └── スライド.md
```

## 🤝 コントリビューション

1. このリポジトリをフォーク
2. 新しいブランチを作成 (`git checkout -b feature/amazing-slides`)
3. 変更をコミット (`git commit -am 'Add amazing slides'`)
4. ブランチをプッシュ (`git push origin feature/amazing-slides`)
5. プルリクエストを作成

## 📜 ライセンス

このプロジェクトはMITライセンスの下で公開されています。
