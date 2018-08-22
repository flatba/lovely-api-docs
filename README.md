# Lovely api documentation



## Setup

aglioをインストール

```
npm install -g aglio
```

## かきかき

* main.md から、各リソースグループごとのmdをincludeしてる
* リソースごとというよりは、機能単位ごとにファイルを分けよう。

```
aglio -i main.md -s
```

で編集中のドキュメントをリアルタイムに http://localhost:3000/ で見ることができる。めちゃ便利。
ポートやホストを変えたいときは `-h 0.0.0.0` とか `-p 8080` とかをつけるとよい。

## HTML変換

```
mkdir -p out
aglio -i main.md -o out/index.html
```

