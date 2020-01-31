# http-mini
[Real World HTTP](https://www.oreilly.co.jp/books/9784873118789/)

## RFC Request For Comment

品質アップのため意見を世界から集める、という名目で仕様を公開した際の名残

## ヘッダ送信

よく使用されるヘッダーに関してはcurlコマンドでエイリアスが用意されている
--user-agent は-A

``````
curl --http1.0 -H "X-Test:Hello" http://localhost:18888
# -v optionで詳細ログ表示
curl -v --http1.0 -H "X-Test:Hello" http://localhost:18888
# POST
curl --http1.0 -X POST http://localhost:18888/greeting
``````
## メソッド

GET サーバに対してヘッダーとコンテンツを要求
HEAD サーバに対してヘッダのみ要求
POST 新しいドキュメントを投稿


