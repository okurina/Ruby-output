# ルーティング
```
<config/routes.rb>
Rails.application.routes.draw do
 get 'posts', to: 'posts#index'
end

get：HTTPメソッド
`posts`：URIパターン
'posts#index'：コントローラー名#アクション名

<ターミナル>
Prefix  Verb  URI Pattern(リクエスト)   Controller#Action(行先)
posts   GET   /posts(.:format)  　　　　posts#index

```
