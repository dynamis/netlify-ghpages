# Netlify GitHub Pages boilerplate

GitHub Pages 同様の変換結果で Netlify にホストするためのボイラープレートです。Markdown ファイルの編集は GitHub Pages 同様にブラウザで編集できるが Netlify の機能を使ってデプロイできるようにするための設定ファイルのテンプレになっています。

ベースとする [GitHub Pages のテーマ](https://github.com/pages-themes/) を選択したら `_config.yml` の theme などを書き換えてご利用ください。必要に応じて [Jekyll Theme のカスタマイズ](https://jekyllrb.com/docs/themes/) や Netlify のリダイレクトやカスタムヘッダなどを組み合わせてご利用ください。

GitHub Pages をそのまま使うのではなく Netlify を使うことで得られるメリットは以下の通り:

- レスポンスヘッダのカスタマイズを _headers で可能
  - キャッシュの制御などやりたいことが GitHub pages ではできないことがある
- リダイレクトを _redirects で指定可能
  - GitHub Pages にはリダイレクト機能はない
- pretty url (.html なしの URL) でアクセス可能に
  - シンプルな URL 
- その他 netlify で提供されている様々な機能

何も考えずに Github Pages のリポジトリを Netlify にホストすると Markdown の変換設定が GitHub Pages と異なり、URL の自動リンクがつかないなどの差異・問題があるため、そのあたりの設定を含めています。

## ファイルリスト

- _config.yml
  - テーマを選択したりサイトのタイトルを設定したりします
  - theme や repository などを書き換えてご利用ください
- _headers
  - netlify のカスタムヘッダ設定ファイル
- _includes
  - Jekyll テーマで利用するインクルードファイルを納めるディレクトリ
  - https://jekyllrb.com/docs/includes/
- _layouts
  - Jekyll テーマで利用するレイアウトファイルを納めるディレクトリ
  - https://jekyllrb.com/docs/layouts/
- _redirects
  - netlify のリダイレクト設定ファイル
- Gemfile
  - github-pages に必要な Gem を指定、インストールさせる
- readme.md
  - このファイル

