---
description: 冷却水の温度が42℃以上を表示している
sidebar_position: 7
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# 水温が高くて加工できない

## HARUKA V0.88～

| 冷却水温度 | フラグ | 動作制限    |
| ----- | --- | ------- |
| 40℃   | 注意  | 加工可     |
| 42℃   | 警告  | 加工不可    |
| 45℃以上 | 警告  | シャットダウン |

## ～HARUKA V0.87

| 冷却水温度 | フラグ | 動作制限    |
| ----- | --- | ------- |
| 30℃   | 注意  | 加工可     |
| 33℃   | 警告  | 加工不可    |
| 35℃以上 | 警告  | シャットダウン |

:::success
<Tabs>
<TabItem value="HAJIME" label="HAJIME">
加工機を休ませて、冷却水の水温を下げる必要があります。また、HARUKA のバージョンが古い場合は V0.88以降にアップデートしてください。
</TabItem>

<TabItem value="HAJIME CL1" label="HAJIME CL1">
加工機を休ませて、冷却水の水温を下げる必要があります。また、HARUKA のバージョンが古い場合は V0.88以降にアップデートしてください。
</TabItem>

<TabItem value="HAJIME CL1 PLUS" label="HAJIME CL1 PLUS">
ヒートシンク
<a href="/docs/process/notoraburu/shinai">フィルターのクリーニング</a>
を勧めます。（取扱説明書 P.54）また、集じん機のフィルターが詰まっている可能性があります。フィルター交換を勧めてください。

高パワーでの長時間加工の場合は水温が上がりやすくなります。

<a href="/assets/水温検証比較表20190910.pdf" target="_blank">水温検証比較表20190910.pdf(PDF)</a>

</TabItem>
</Tabs>
:::

:::note 外部リンク
[MIRUKU メンテナンスマニュアル(PDF)](https://www.oh-laser.com/files/miruku_maintenance.pdf) 
:::
