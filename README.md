### ルール

- 本を読んで重要だなと思ったところを記載する
- 仕事関係は/workに、個人的なものは/privateに置く
- 本の題名でissuesを立てて、`is{issue番号}`のブランチを切る（例：issues#11の場合、is11）
- ファイル名は「本の名前\_yyyymm.md」にする
  - Github actionsでファイル名チェックする
- 見出しは#3つで統一する
- Node23.xを使用する(`nvm install`)
  - Textlintで文章のリントをする
  - Prettierで全ファイルformatする
    - `npm run format`
    - pre commitで走るけども
  - ライブラリはRenovateで自動管理する
