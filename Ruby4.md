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
