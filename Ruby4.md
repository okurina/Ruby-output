# フォーム
```
<h1>新規投稿ページ</h1>

<form action="/posts" method="post">
  <input type="text" name="content">
  <input type="submit" value="投稿する">
</form>

action属性・・・リクエスト先のURLを指定する　⇒　localhost:3000/postsへ
methot属性・・・リクエストに使用されるHTTPメソッドを指定する属性　⇒　method="post"　POSTを指定している
```
# form_withメソッド(Rails:ヘルパーメソッド)
```
<form action="/posts" method="post">
  <input type="text" name="content">
  <input type="submit" value="投稿する">
</form>
↓
<%= form_with url: "/posts", method: :post, local: true do |form| %>
  <%= form.text_field :content %>
  <%= form.submit '投稿する' %>
<% end %>

localオプション・・・リモート送信(Ajax通信)を無効にするかどうかを指定。trueは無効になる
text_field・・・1行のテキストボックス
password_field・・・パスワード入力ボックス
check_box・・・チェックボックス（複数選択可）
radio_button・・・ラジオボタン（複数の中から1つ選択）
submit・・・送信ボタン
※submit以外はキー(:~)が必要

```
