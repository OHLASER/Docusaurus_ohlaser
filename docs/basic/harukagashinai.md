---
description: 情報漏えい対策ソフトで USBデバイスが制御され HAJIME とドングルが認識されない
---

# USBポート制限ソフト

## USBポート制御ソフトを削除

**不具合を確認しているパソコンメーカー製のUSBポート制御ソフト**

* HP ProtectTools（デバイスへのアクセス制限 ～ Device Access Manager ～との相性問題）
* Dell Data Protection Security Tools（USB 接続機器の監視）

:::caution
過去に上記ソフトが HAJIME とドングルを遮断している事がありました。
:::

**その他に不具合を起こしそうなソフト**

* Endpoint Protector（エンドポイントプロテクター）
* Portshutter （ポートシャッター）
* Malion Cloudなど

:::success
**削除が可能な場合**

1. USB制御ソフトのアンインストール
2. HARUKA のアンインストール
3. パソコンの再起動
4. HARUKA の再インストール
5. USB ケーブルの抜き差しまたは、接続口の変更

以上を行い、再度接続状況を確認します。

**削除ができない場合**

1. ホワイトリストにHAJIMEとドングルを登録します。
2. ホワイトリストへの登録ができない場合は、別途USB制御ソフトが入っていないパソコンを用意していただき、HARUKA をインストールして接続状況を確認をしてください。
:::

