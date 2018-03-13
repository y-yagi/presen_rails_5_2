### [Content Security Policy](https://github.com/rails/rails/pull/31162)

* javascript_tagメソッドでnonceが使えるようになっている

```ruby
<%= javascript_tag nonce: true do %>
  alert('Hello, World!');
<% end %>
```

* これにより、inlineでのJavaScriptを禁止している場合も、一部のJSだけ実行、という事ができる
  * rails-ujsはこれを使っている
