FORMAT: 1A

# Group 【APP】todo

## 取得 [GET /api/v1/todos/:id]

    todoの取得

+ Response 200 (text/plain)

        Hello World!

## 登録 [POST /api/v1/todos/:id]

    todoの取得

+ Response 200 (text/plain)

        Hello World!

## 取得 [GET /api/v1/todos]

    todo一覧の取得

+ Response 200 (text/plain)

## Example Response
```json
{
    "success": true,
    "todos": [
    {
        "id": 3,
        "title": "きっとお気に入りのお店になる。恵比寿「GOOD LUCK CURRY」が話題",
        "text": "一向に涼しくなる気配のない今年の夏。そんな暑すぎる夏についつい食べたくなる、東京近郊のアイスクリーム屋さんをご紹介します。美味しい＆お洒落なひんやりスイーツを食べて猛暑を乗り切りましょう！（※掲載されている情報は2018年8月記事公開時点のものです。必ず事前にご確認ください。）",
        "background_color": "#ff69b4",
        "background_image_url": "https://www.irasutoya.com/2018/10/blog-post_638.html",
        "completed": false,
        "user_id": 3,
        "created_at": "2018-10-15T15:51:05.599Z",
        "updated_at": "2018-10-15T15:51:05.599Z",
        "position": 1,
        "couple_id": 2
    }
    ]
}
```

## 更新 [PATCH /api/v1/todos/:id]

    todoの削除

+ Response 200 (text/plain)

        Hello World!
