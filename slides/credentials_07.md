### [encrypted](https://github.com/rails/rails/commit/68479d09ba6bbd583055672eb70518c1586ae534)

* credentialsコマンドとは別にencryptedコマンドも実は入った
* credentialsと異なり、設定ファイルや暗号に使用するkeyをコマンドで指定することが出来る
* 環境ごとに異なる秘匿情報を扱いたい場合に使うように追加された(PR出した人の思いとしては)
