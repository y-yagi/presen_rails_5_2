### [Content Security Policy](https://github.com/rails/rails/pull/31162)

* Content Security Policy headerを設定出来るよう対応
  * Content Security Policyについては [Content Security Policy \(CSP\)](https://developer.mozilla.org/ja/docs/Web/Security/CSP) を参照
* 設定はアプリ全体(initializersで実施)、及び、controller単位で出来るようになっている
* 色々問題があってデフォルトでは無効にされている
