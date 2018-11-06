# API
## 基本方針
- RESTfulとCRUDに準拠する
- SSDKsなAPIなので、chattyにならないように関連データも含める
- 必要に応じてオーケストレーションもしていく

### レスポンス
- `POST` は status `201` でbodyに追加したデータを返却
- `PUT` `PATCH` はstatus `200` でbodyには変更したデータを返却
- `DELETE` はstatus `204` を返却する。 bodyには何も含めない
- 基本的にRFCに準ずる

### エラーについて
APIエラーが起こった際は、適切なステータスコードを指定した上で、
下記のようにエラー詳細をbodyに含めて返却する

#### response

```
  {
    code: string,
    details: array or string
  }
```

### ※注意事項
- REST URLで表現している(:id)などは `request` 内のオブジェクトには含みません

# Login
### POST /api/users/login ログイン
#### request
```
  //  WIP
  {
      email: string,
      password: string
  }
```

#### response

```
  //  WIP
  {
    access_token: string,
  }
```
---

# User

## SHOW /api/user/:id

#### request

```
  {}
```

#### response

```
  //  WIP
  {
    name: string,
  }
```
---
