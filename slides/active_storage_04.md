### Active Storage

* model毎にカラムを追加するのではなく、すべてのファイルを同じテーブルで管理する(管理用のテーブルは2つ)
* active_storage:install  というタスクを実行するとstorge用のmigrationファイルが生成されるので、後はdb:migrateを実行すればOK

