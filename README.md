# sample_app

Rails チュートリアルのサンプルアプリケーションです  
内容は第4版の第3章以降 ( https://railstutorial.jp/?version=5.0#walk-through )  

### 事前準備

- rubyをローカルに入れる
- ruby 2.4は動作確認済み

### 動作確認方法

- ソースをクローン

```
$ git clone https://github.com/masa-nakano/sample_app.git
```

- gemを入れる

```
$ bundle install --path vendor/bundle
```

- DBをmigrateして動作確認用のデータを投入

```
$ bundle exec rails db:migrate
$ bundle exec rails db:seed
```

- ローカルでサーバーを立ち上げる

```
$ bundle exec rails s
```

- ブラウザから http://localhost:3000/ に接続

- 画面右上の Log in から以下のユーザーでログイン

```
Email: example@railstutorial.org  
Password: foobar  
```

<br />

### その他

- developmentのDBはsqliteを使用しています。  
- prodction用のherokuの設定は行っていません。  
