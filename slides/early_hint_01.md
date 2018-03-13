### [HTTP/2 Early hints support](https://github.com/rails/rails/pull/30744)

* HTTP/2のEarly Hintsのサポートをjavascript_include_tag、stylesheet_link_tagメソッドに追加
  * Early Hints については、[HTTP の新しいステータスコード 103 Early Hints](https://blog.jxck.io/entries/2016-12-16/103-early-hints.html) とか [Implementing Early Hints in Chrome](https://www.slideshare.net/VietHoangTran/implementing-early-hints-in-chrome)参照
* デフォルトだとオフになっていて、サーバ起動時に`--early-hints`オプションを指定する必要がある
* Puma(3.11.0 以降)じゃないと今のところ動かない
  * Early Hints用のrack header(`rack.early_hints`)の対応が入っているのがPumaだけな為
