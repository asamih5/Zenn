---
title: "JavaScriptでカラーピッカーを作成する" # 記事のタイトル
emoji: "🎨" # アイキャッチとして使われる絵文字（1文字だけ）
type: "tech" # tech: 技術記事 / idea: アイデア記事
topics: [JavaScript] # タグ。["markdown", "rust", "aws"]のように指定する
published: false # 公開設定（falseにすると下書き）
---
## はじめに
JavaScript学習のためにカラーピッカーを作成しました。

この記事は、WebクリエイターボックスManaさんの「1冊ですべて身につくJavaScript入門講座」の内容を引用しています。
https://www.sbcr.jp/product/4815615758/

## デモ
@[codepen](https://codepen.io/asamih5/pen/qBLrVjr)

## 色の値を取得する
HTMLのinputタグにつけた、「colorPicker」というIDからカラーコードを取得します。
「querySelector()」のメソッドを使い、HTMLの中から任意のIDがついた要素を取得し、「.value」でその値を取得します。取得できているか確認するため、一旦コンソールに表示します。
```html:index.html
<input id="colorPicker" type="color">
```
```js:script.js
console.log(document.querySelector('#colorPicker'));
```
