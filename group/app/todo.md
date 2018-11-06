FORMAT: 1A

# Group 【APP】todo

## 登録 [POST /api/v1/todos

    Todoの作成

    + Headers

    ```
        content-type: application/json
        token-type: Bearer
        access-token: 5ODLOGYKvlM0OvcUXdmcBQ
        uid: test_men@lovely.com
        client: C_adlx6ZxZdbHk3mfJRHLQ
    ```

    + Body

    ```
        {
            "title": "ポストしてTODOつくる！！",
            "text": "これはTODO作成機能のテストです。",
            "background_color": "#ff69b4",
            "background_image_url": "https://www.irasutoya.com/2018/10/blog-post_638.html",
            "completed": "false",
            "user_id": "3",
            "couple_id": "4"
        }
    ```

+ Response 200 (text/plain)

        Hello World!

## 取得 [GET /api/v1/todos]

    Todoの取得

    + Response 200 (application/json)

    + Headers

    ```
        content-type: application/json
        token-type: Bearer
        access-token: 5ODLOGYKvlM0OvcUXdmcBQ
        uid: test_men@lovely.com
        client: C_adlx6ZxZdbHk3mfJRHLQ
    ```

+ Response 201 (text/json)

+ Response example ユーザー名変更 (application/json)

    + Body

    ```json
        {
        "code": "201",
        "details": {
        "todo": [
                    {
                    "id": 4,
                    "title": "きっとお気に入りのお店になる。恵比寿「GOOD LUCK CURRY」が話題",
                    "text": "これはテストです．",
                    "background_color": "",
                    "background_image_url": "",
                    "completed": false,
                    "user_id": 3,
                    "created_at": "2018-11-03T07:17:27.691Z",
                    "updated_at": "2018-11-03T07:17:27.691Z",
                    "position": 1,
                    "couple_id": 4
                    },
                    {
                    "id": 5,
                    "title": "今夜は2人きりで。夜を120％楽しむ、大人のドライブデート先10選",
                    "text": "これはテストです．",
                    "background_color": "",
                    "background_image_url": "",
                    "completed": false,
                    "user_id": 3,
                    "created_at": "2018-11-03T08:13:50.234Z",
                    "updated_at": "2018-11-03T08:13:50.234Z",
                    "position": 2,
                    "couple_id": 4
                    },
                ],
            }
        }
    ```


## 更新 [PATCH /api/v1/todos/:id]

    todoの更新

+ Response 201 (application/json)

    + Headers

    ```
        content-type: application/json
        token-type: Bearer
        access-token: 5ODLOGYKvlM0OvcUXdmcBQ
        uid: test_men@lovely.com
        client: C_adlx6ZxZdbHk3mfJRHLQ
    ```

    + body

    ```
        {
            "title": "ドン・キホーテもびっくり！魅惑の釜飯で夕食をドンッ！",
            "text": "鳥スープがおすすめとのこと！",
            "background_color": "#FE642E",
            "background_image_url": "https://www.irasutoya.com/2018/10/blog-post_638.html",
            "completed": "true",
            "user_id": "3",
            "couple_id": "2"
        }
    ```

+ Response 201 (text/json)

+ Response example ユーザー名変更 (application/json)

    + body

    ```
        {
            "title": "ドン・キホーテもびっくり！魅惑の釜飯で夕食をドンッ！",
            "text": "鳥スープがおすすめとのこと！",
            "background_color": "#FE642E",
            "background_image_url": "https://www.irasutoya.com/2018/10/blog-post_638.html",
            "completed": "true",
            "user_id": "3",
            "couple_id": "2"
        }
    ```


## 削除 [DELETE /api/v1/todos/:id]

+ Response 204 (text/plain)

    + Headers

    ```
        content-type: application/json
        token-type: Bearer
        access-token: 5ODLOGYKvlM0OvcUXdmcBQ
        uid: test_men@lovely.com
        client: C_adlx6ZxZdbHk3mfJRHLQ
    ```

+ Response 204 (text/plain)
