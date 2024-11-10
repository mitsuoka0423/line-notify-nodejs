# LINE Notify Node.js

> [!WARNING]
> このリポジトリはLINE Notifyのサービス終了に伴い、アーカイブされます。  
> This repository will be archived due to the closure of the LINE Notify service.
>
> > https://notify-bot.line.me/closing-announce

LINE Notify APIのNode.jsライブラリです。


<a href="https://www.buymeacoffee.com/mitsuoka0423"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=mitsuoka0423&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" width="150px" /></a>
>
> 開発の励みになりますので、使ってみて便利でしたらコーヒーをご馳走してください

## Install

```
$ npm install line-notify-nodejs
```

## How to Use

1. 下記ページでトークンを発行する
    - https://notify-bot.line.me/my/

2. トークンを使用して通知を送信する

```javascript
const lineNotify = require('line-notify-nodejs')('LINE NOTIFY TOKEN HERE');

lineNotify.notify({
  message: 'send test',
}).then(() => {
  console.log('send completed!');
});
```
