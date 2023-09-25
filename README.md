# Sample App for Learning Debug
デバッグ講義用サンプルアプリ

## インストールと起動
1.下記のコードを入力して、アプリケーションを起動できるようにします。
```
$ bundle install
$ yarn install
$ rails db:migrate
$ rails db:fixtures:load
```
※ `rails db:fixtures:load` は予め用意したテストデータを読み込むコマンドの1種です。

2.`config/environments/development.rb`にご自身のホスト設定を追記してください。
```ruby
require "active_support/core_ext/integer/time"

Rails.application.configure do
  :
  :
  config.hosts << "xxxx.vfs.cloud9.ap-northeast-1.amazonaws.com"
end
```

3.`rails s`を実行して、Yay! You're  on Rails!と表示されたら準備完了です
