![img](./src/static/static/images/opengraph.png?raw=true)

# みんなの63

これは「みんなの63 - スクリーンショットから自動解析できるポケモンの選出投稿サイト」の開発レポジトリです。

## Installation

### Environment Varialbles

Firebase のプロジェクトを用意して設定してください。

手軽に確認したい場合、テスト用に用意している Firebase プロジェクトがあるため、`cp .env.sample .env` にて、以下を設定ください。

```.env
FIREBASE_API_KEY="AIzaSyB-Jh74U8rwbQq6sMyLTliOamXhGyE3U2g"
FIREBASE_AUTH_DOMAIN="minnano63-dev.firebaseapp.com"
FIREBASE_DATABASEURL="https://minnano63-dev.firebaseio.com"
FIREBASE_PROJECT_ID="minnano63-dev"
FIREBASE_STORAGE_BUCKET="minnano63-dev.appspot.com"
FIREBASE_MESSAGING_SENDER_ID="924539713345"
FIREBASE_APP_ID="1:924539713345:web:a5ab68eff31fcab88b53c0"
FIREBASE_MEASUREMENT_ID="G-SJ4HEZYE1T"
```

Hosting へのデプロイやセキュリティルールの設定などはできませんが、全てが読み書きできる状態で開放されています。

### Image assets

pokesprite の画像を利用する場合、以下で有効化できます。

```
$ cd src/static
$ mkdirp pokemon63
$ cd pokemon63
$ cp ./node_modules/pokesprite-images/pokemon-gen8/regular/*.png ./src/static/static/imagse/icons/
$ ln -s ../static/ ./static/
```

### Server

```bash
$ yarn
$ yarn dev
$ open 'http://localhost:3000/pokemon63/'
```

## LICENCE

MIT
