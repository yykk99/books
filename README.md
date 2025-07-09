### ルール

- 本を読んで重要だなと思ったところを記載する
- 仕事関係は/workに、個人的なものは/privateに置く
- ファイル名は「本の名前\_yyyymm.md」にする
- 見出しは#3つで統一する
- Node23.xを使用する(`nvm install`)
  - Textlintで文章のリントをする
  - Prettierで全ファイルformatする
    - `npm run format`
    - pre commitで走るけども
  - ライブラリはRenovateで自動管理する
- Github actionsでファイル名チェックする
