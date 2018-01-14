### Active Storage(前回からのアップデート)

* `rails new`時にActive Storage用のmigrationファイルを生成しなくなった
  * Active Storageを使いたい場合、明示的に`active_storage:install`を実行したmigrationファイルを生成する必要がある
  * あと使いたいクラウドサービス用のgemを自分でGemfileに指定する必要がある(`aws-sdk-s3`、`google-cloud-storage`等)
* Preview機能が入った
