# echo_training

- golang echoの練習用

## イメージ

- user:会員的な存在
  - user_id
  - name
  - service
- service:サービス的な存在
  - 次に入れる

## uri

- http://[ServerIP]/[uri]

|     API     |       URI        | Method |              option              |               目的               |
| ----------- | ---------------- | ------ | -------------------------------- | -------------------------------- |
| get_user    | /users/[ID]      | GET    |                                  | GETとURIからIDを拾う             |
| search_user | /users?name=hoge | GET    |                                  | クエリから条件を拾う             |
| add_user    | /users           | POST   | json形式でbodyに会員情報を入れる | POSTとbody読み取りとjsonデコード |
| change_user | /users           | PUT    | json形式でbodyに会員情報を入れる | PUTで変更                        |
| delete_user | /users/[ID]      | DELETE |                                  | DELETEで削除                     |

## DB

- はあとで
- とりあえずオンメモリで展開することにする