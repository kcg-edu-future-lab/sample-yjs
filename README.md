# sample-yjs

[yjs](https://github.com/yjs/yjs)を利用した共同編集のサンプルアプリです。[yjs-demos](https://github.com/yjs/yjs-demos)のcodemirrorサンプルのコードを独自にビルドしてcodemirror.bundle.jsを生成し、それを利用しています。

サーバは https://fungo.kcg.edu/yjs を利用しています。

yjsでは、[CRDT(Conflict-free Replicated Data Type)](https://hal.inria.fr/hal-00932836/file/CRDTs_SSS-2011.pdf)という
データ共有技術が実装されています。


## 起動方法

まず、このリポジトリをcloneしてください。

```
git clone https://github.com/kcg-edu-future-lab/sample-yjs
```

次に、Python3を使ってwebサーバを立ち上げてください。

```
cd sample-yjs
python3 -m http.server
```

ブラウザで以下のURLにアクセスすると，共同編集のデモが表示されます。
同じタイミングで誰かがデモを表示していると，編集内容が共有されます。

* http://localhost:8000/

![利用イメージ](screenshot.gif)
