### [Add preload_link_tag helper](https://github.com/rails/rails/pull/31251)

* rel="preload" によるコンテンツの先読みを行う為のメソッド
  * preloadについては、[rel="preload" によるコンテンツの先読み](https://developer.mozilla.org/ja/docs/Web/HTML/Preloading_content) とか [resouce hintsとpreloadを使ってリソースの取得を最適化する](https://blog.kazu69.net/2016/03/19/optimize_resources_using_resoucehint_and_preload/)参照

```ruby
preload_link_tag(post_path(format: :json), as: "fetch")
# => <link rel="preload" href="/posts.json" as="fetch" type="application/json" />
```

* ここでもEarly Hintsが使われている(リクエストがあればEarly Hintsを送信するようになっている)
