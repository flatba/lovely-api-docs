# Lovely api documentation

- ID "lovely"
- password "lovely0519"
- https://hip-lovely-api-docs.herokuapp.com/

## Setup

aglioをインストール

```
npm install -g aglio
```

## かきかき

* main.md から、各リソースグループごとのmdをincludeしてる
* リソースごとというよりは、機能単位ごとにファイルを分けよう。

group/app下のファイルをそれぞれ編集する
書き方のフォーマットがあるみたい。
https://apiblueprint.org/

```
aglio -i main.md -s
```

で編集中のドキュメントをリアルタイムに http://localhost:3000/ で見ることができる。めちゃ便利。
ポートやホストを変えたいときは `-h 0.0.0.0` とか `-p 8080` とかをつけるとよい。

## HTML変換

Markdownのファイルを編集したら、下記のコマンドを実行して、htmlファイルを生成してgithubにpushする。

```
aglio -i main.md -o public/index.html
```

