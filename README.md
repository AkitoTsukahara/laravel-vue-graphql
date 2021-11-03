```
$ docker-compose up -d
```

3.以下のコマンドで php コンテナに入ります。

```
$ docker-compose exec php bash
# 不要なファイルを削除します
$ rm .gitkeep
```

4.laravel のプロジェクトを立ち上げましょう！

```
# バージョンを指定しない場合
$ composer create-project --prefer-dist laravel/laravel ./
# バージョンを指定する場合
$ composer create-project --prefer-dist laravel/laravel=8.* ./
```

5.`http://localhost/`で Laravel のウェルカムページが表示されたら成功です!  
止めたい時は以下のコマンドを入力してください。

```
$  docker stop $(docker ps -q)
```
