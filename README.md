# gf-tsutenkaku
## 
This document is for [gitfab](http://gitfab.org)
---
#ムービ

---
#概要
ウェブブラウザでも情報を見ることはできますが、同じ情報でも実世界に取り出し表現することで、また違った感覚を得ることはできそうな気がします。tsutenkaku は、通天閣の写真に組み込まれたマルチカラーのLEDから、閲覧中のウェブページの地域性(大阪限定)と、そこの明日のお天気を緩やかに知覚するコトができるアプリケーションです。とてもシンプルですが、ウェブ内情報を見るという意味では、これも一つのウェブブラウザであると言えるのかもしれません。
---
#Firefox Addon のセットアップ

[tsutenkaku.xpi](https://raw.github.com/dadaa/gf-tsutenkaku/master/materials/tsutenkaku.xpi) を Firefox でクリックしてください。インストールが始まります。
---
#Arduino のセットアップ
[CommandServer.ino](https://raw.github.com/dadaa/arduino.js/master/core/sketch/CommandServer/CommandServer.ino) を Arduino にアップロードしてください。
---
#ハードウェアのセットアップ
利用する部品

* Arduino
* マルチカラーLED
* 抵抗100Ω x 2
* 抵抗150Ω x 1
* ブレッドボード
* ジャンパー線

![hardware.JPG](https://raw.github.com/dadaa/gf-tsutenkaku/master/materials/hardware.JPG)

※ほんとは回路図を入れるんでしょうね。
---
#使い方

---
#実装の話
ハード面の実装はとてもシンプルです。お気に入りの通天閣の写真(CCライセンスが付いているのが良いです)にマルチカラーの LED を裏側から挿し込みます。マルチカラーLED には４つの端子が出ておりますが、ここで利用した LED では、一つはグラウンド、あとの３つはそれぞれ RGB に割り当てられていました。これらをワニ口クリップでくわえ、抵抗を通し、Arduino の然るべき PIN に接続します。
ソフトウェアは arduino.js を利用したアドオンとして実装しました。LED 点灯のスイッチは、閲覧中のウェブページの URL に osaka が入っているか否かで切り替えています。また LED の色が明日の天気予報になっていますが、天気予報は Yahoo Japan さんのお天気RSSを取得し決定しています。ちなみに本来の通天閣の色は 白→晴、橙→曇、青→雨 となっており、晴時々曇ですと、上段が白、下段が橙に光ります。本アプリでは、緑→晴、赤→曇、青→雨とし、時間軸でその色を変化させるコトにしました。
---
#参照サイト
* [ホームページ](http://www.mecha-mozilla.org/projects/tsutenkaku/)
* [tsutenkaku Addon ソースコード](https://github.com/dadaa/tsutenkaku)
---
