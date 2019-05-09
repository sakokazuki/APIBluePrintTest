# GET /message{?text}
パラメーター"text"にテキストを入れてリクエストをするとjsonを返す。
テキストが空の場合、400エラーを返す。

+ Parameters
  + text (string) - メッセージ

+ Response 200 (application/json)
        {
          "text": "メッセージ メッセージ メッセージ",
          "image": "https://XXXXXXXXX/image.jpg"
        }
        
+ Response 400 (application/json)  
        {
          "message": "不正なメッセージです。" 
        }
      