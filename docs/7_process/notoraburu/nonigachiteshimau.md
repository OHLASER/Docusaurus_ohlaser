---
description: 加工中に電源が落ちLED電源ボタンが高速点滅
sidebar_position: 7
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# 加工途中に電源が落ちる

## **安全装置が働き電源が落ちています**

* 加工中に水流、水温の異常を検知した
* 加工中にフタの開放を検知した
* 加工中に加工エリアのリミットを検知した

以上に関わるステータスエラーの検知や、各センサー部品の故障が考えられます。

## HARUKAのステータスを確認します

### **1.加工中に「水流：低下、停止」が表示した場合**

:::info
待機時（加工開始前）は「水流：停止」と表示されます。（異常ではありません）
:::

:::success
<Tabs>
<TabItem value="HAJIME" label="HAJIME">
冷却水に問題があるかもしれません。水量の確認、交換、
<a href="/docs/process/notoraburu-1/garanai/gattekara15guraidechiru">ウォータータンクのクリーニング</a>
を行ってください。また、フローセンサーの信号を、HARUKA が正しく受け取れていない可能性があります。
<a href="/docs/soft/harukanomkugarishitsuitarietarisuruusbnogarishiru">USB 接続</a>
環境を確認してください。

上記を行っても回復しない場合は、フローセンサー、ウォーターポンプが故障しています。交換修理が必要です。
</TabItem>

<TabItem value="HAJIME CL1" label="HAJIME CL1">
冷却水に問題があるかもしれません。水量の確認、交換、
<a href="/docs/process/notoraburu-1/garanai/gattekara15guraidechiru">ウォータータンクのクリーニング</a>
を行ってください。また、フローセンサーの信号を、HARUKA が正しく受け取れていない可能性があります。
<a href="/docs/soft/harukanomkugarishitsuitarietarisuruusbnogarishiru">USB 接続</a>
環境を確認してください。

上記を行っても回復しない場合は、フローセンサー、ウォーターポンプが故障しています。交換修理が必要です。
</TabItem>

<TabItem value="HAJIME CL1 PLUS" label="HAJIME CL1 PLUS">
フローセンサーの信号を、HARUKA が正しく受け取れていない可能性があります。
<a href="/docs/soft/harukanomkugarishitsuitarietarisuruusbnogarishiru">USB 接続</a>環境を確認してください。

USB 接続環境に問題が無い場合は、フローセンサー、ウォーターポンプが故障しています。交換修理が必要です。
</TabItem>
</Tabs>
:::

### **2.水温が45℃以上を表示している場合**

|         |       |         |
| ------- | ----- | ------- |
| 40℃　　　　 | 注意　　　 | 加工可     |
| 42℃     | 警告    | 加工不可    |
| 45℃ 以上  | 警告    | シャットダウン |

:::success
<Tabs>
<TabItem value="HAJIME" label="HAJIME">
加工機を休ませて、冷却水の水温を下げる必要があります。
</TabItem>

<TabItem value="HAJIME CL1" label="HAJIME CL1">
加工機を休ませて、冷却水の水温を下げる必要があります。
</TabItem>

<TabItem value="HAJIME CL1 PLUS" label="HAJIME CL1 PLUS">
ヒートシンク
<a href="/docs/process/notoraburu/shinai">フィルターのクリーニング</a>
を勧めます。（取扱説明書 P.54）また、MIRUKUのフィルターが詰まっている可能性があります。フィルター交換を行ってください。
</TabItem>
</Tabs>
:::

:::note 外部リンク
[MIRUKU メンテナンスマニュアル(PDF)](https://www.oh-laser.com/files/miruku_maintenance.pdf) 
:::

### **3.フタを閉じているのに「フタ：開いてます」が表示する場合**

:::caution
インターロックスイッチの信号を、HARUKA が正しく受け取れてない可能性があります。
:::

### **4.加工途中に「加工エリアを超えています」が表示する場合**

:::caution
彫刻データが 490mm x 300mm 以上で作られている場合、レーザーヘッドがMAXリミットに接触するため、電源が落ちます。

または、リミットスイッチからの信号を、HARUKA が正しく受け取れてない可能性があります。
:::

## 本体とパソコンとの通信状況が悪い可能性があります

各センサーからの信号を、HARUKA が正しく受け取れていない場合は下記を確認してください。

:::success
**USB 差し込み口が原因**

* パソコン側のUSB 差込口を別の場所にしてみる。何度か差し直してみる。
* バスパワーの USB ハブを使用していないか確認する。（バスパワーのハブは通信不良になる可能性があります。セルフパワーなら大丈夫。）

**ケーブル不良が原因**

* 2m以上のケーブルを使用していないか確認する。（長いケーブルは通信不良になる可能性があります。2m以内にしてください。）
* ケーブル自体が断線していないか確認する。（別のものに交換　※ごくまれにあります）

**パソコンが原因**

* HARUKA の[システム条件](/docs/basic/pc_spec)に合っているパソコンか確認する。
* [セキュリティーソフト](/docs/soft/harukaganishinai/sekyuritsofutono)で通信を監視、遮断されていないか確認する。
:::

:::note 外部リンク
[Amazon.co.jp: エレコム USB3.0 ハブ 4ポート 1ｍ ACアダプタ付 セルフ/バス両対応 MacBook / Surface Pro / Chromebook他 ノートPC Nintendo Switch対応 ブラック U3H-A408SBK : パソコン・周辺機器](https://www.amazon.co.jp/dp/B00KKJJCXC/?coliid=I9R7OGQUCPEL4&colid=2P27YP4M43BSD&psc=1) 
:::

## メイン基板が誤動作している可能性があります

:::success
主電源をオフにして、背面のケーブル類をすべて抜き数分間放置します。 その後ケーブルを繋いで再起動をお願いします。

[アース接地の確認](/docs/basic/earth)をします。
:::

:::danger
以上の確認をしても症状が回復しない場合は修理対応になります。

*   **水流：低下、異常**

    * フローセンサーの故障
    * ウォーターポンプの故障
    * メイン基板、発振器電源の故障


*   **フタ：開いてます**

    * インターロックスイッチの故障
    * メイン基板、発振器電源の故障


* **作業エリアを超えています**
  * MAXリミットスイッチの故障
  * メイン基板、発振器電源の故障
:::

## ステータスエラーがない場合

特にステータスエラーの表示がない場合も、念のためパソコンとの通信状況を確認してください。

:::danger
アース接地の接続やパソコン環境を整えても症状が回復しない場合は、メイン基板の故障、内部ケーブルの故障が考えられます。（アース接地を行わずに長期間運転した場合、基板にノイズが帯電し続けて故障する可能性があります。）
:::
