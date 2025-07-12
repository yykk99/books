### 環境構築

- 前提
  - nvmがインストールされていること
  - vscodeで`.vscode/extensions.json`の拡張機能をインストールしていること

- 必要パッケージインストール

  ```
  $ nvm install
  $ npm i
  ```

- おわり

### 技術構成

- Node.js(nvm)
  - textlint(文章のリンター)
  - prettier(フォーマッター)
  - husky(pre commitでフォーマッターを走らせる)

- Github Actions
  - filename-check
    - ファイルが{本の題名\_yyyymm.md}かチェックする
  - textlint
    - textlintを実行し、失敗した場合PRにエラー内容を表示する

- Renovate
  - Node.js、ライブラリのバージョンアップを検知し自動でPRを作る

### 運用ルール

1. まとめたい本の題名でissueを作る
1. issueの番号でPRを切る
1. {本の題名\_yyyymm.md}のファイル名で/workまたは/privateに作成する
1. まとめが完了している && ciが通っていればマージする

#### 細かいこと

- issue、PRにはラベルをつける(work/private/fix)
- 見出しは###を使用する
