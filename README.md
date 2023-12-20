# Suumo_test
Suumo scraping


####実施内容####
#・取得情報 \n
#　東京駅20分圏内の賃貸物件(物件数が多く5ページまでの集約)
#　'物件名', '住所', '最寄り駅1-3', '築年数', '総階数', '部屋の階数', '家賃', '管理費', '敷金', '礼金', '間取り', '専有面積'

#・Python
#データ取得
#　Selenium
#　Webdriver(今回はブラウザ非表示(Option))
#　データ収集段階で2,712件の物件情報
#　重複削除用にCheck列を作成(住所+築年数+階数+間取り+専有面積)
#重複削除
#　重複削除後のデータを集計(drop_duplicates)
#　Check列から重複削除
#　削除後のデータは331件
#Googleスプレッドシート
#　お決まりの2行
#　scope = ['https://www.googleapis.com/auth/spreadsheets','https://www.googleapis.com/auth/drive']
#　credentials = Credentials.from_service_account_file("-------------json URL----------------", scopes = scope)
#　シート指定→データ入力

