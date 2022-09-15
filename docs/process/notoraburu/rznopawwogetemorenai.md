---
description: レーザーは出るが前より弱くなった
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# レーザーが弱い・切れない

## 光学部品の汚れ

![](/assets/20191112\_03.jpg)

光学部品の汚れが原因でレーザーパワーが弱くなっている可能性があります。特にフォーカスレンズ裏側のクリーニングが出来ていない場合が多いので、確認してください。（取扱説明書 P.52）

{% embed url="https://www.oh-laser.com/files/plus_maintenance.pdf" %}

{% embed url="https://www.amazon.co.jp/ガレージ・ゼロ-イソプロピルアルコール-2-プロパノール-イソプロパノール-GZ900/dp/B01AJ1XWHM/ref=lp_3450764051_1_1_sspa?s=industrial&ie=UTF8&qid=1571809764&sr=1-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFSQThMMUJEWUxGME8mZW5jcnlwdGVkSWQ9QTA4NTg0MjNVSEIzWlJCQU5QSk0mZW5jcnlwdGVkQWRJZD1BVEVBODNFVk5CTFpKJndpZGdldE5hbWU9c3BfYXRmX2Jyb3dzZSZhY3Rpb249Y2xpY2tSZWRpcmVjdCZkb05vdExvZ0NsaWNrPXRydWU=" %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}



## 水温の上昇

冷却水の温度が上昇して発振器が熱くなると、レーザーパワーが減少します。

![冷却水が40℃に到達すると、レーザーパワーが約25%（10W）減少します。](/assets/hajime\_cooling\_03.png)

:::success
<Tabs>
<TabItem value="HAJIME" label="HAJIME">
加工機を休ませるか冷却水を冷たい水に交換して様子を見てください。
</TabItem>

<TabItem value="HAJIME CL1" label="HAJIME CL1">
加工機を休ませるか冷却水を冷たい水に交換して様子を見てください。
</TabItem>

<TabItem value="HAJIME CL1 PLUS" label="HAJIME CL1 PLUS">
排気効率が落ちている可能性があるので、ヒートシンク[フィルターのクリーニング](shinai.md)を勧めてください。（取扱説明書 P.54）また、集じん機のフィルターが詰まっている可能性もあるので、確認してください。
</TabItem>
</Tabs>
:::

{% embed url="https://www.oh-laser.com/files/miruku_maintenance.pdf" %}

本体背面コンセントの排気ファンとコンプレッサーの差し込み位置が逆になっていると、加工終了後すぐに排気ファンが止まってしまい冷却できません。間違っていないか確認してください。

![](/assets/haruka\_splash\_04.png)

## フォーカスずれ

レーザーヘッドにあるフォーカス調整ネジ（白いユリアネジ）が加工中に緩んでしまい、フォーカスがずれてしまっている可能性があります。締め付けを確認してください。

また、加工中に素材が反ってしまい、フォーカスがずれてしまっている可能性があります。再度反りに合わせてフォーカスを調整してください。

:::caution
フォーカスがずれたまま加工をすると、素材が発火しやすいので注意が必要です。HAJIME の標準フォーカスレンズの焦点深度（焦点が合っている有効距離）は、約1.5mmです。
:::

## 素材密度のばらつき

木材やベニヤ板などは木目のスジなどの細胞が詰まっている箇所と、空気が通っている箇所があり素材密度が均等ではありません。綺麗に切りぬけない場合が多いのでご理解ください。

{% content-ref url="../../adobaisu/adobaisu/ha/beniya.md" %}
[beniya.md](../../adobaisu/adobaisu/ha/beniya.md)
{% endcontent-ref %}

## レーザー発振器の消耗

以上の項目に問題がない場合は、発振器内部の炭酸ガスが消耗し劣化している可能性があります。

:::danger
レーザー発振器の交換修理になります。
:::

## ハニカムテーブルのゆがみ
