---
description: HARUKA の動作に必要な Microsoft のコンポーネントがパソコンにインストールされていない
sidebar_position: 8
---

# api-ms-win-crt-runtime-l1-1-0.dll

## 考えられる原因

### 「api-ms-win-crt-runtime-l1-1-0.dllがない」または「api-ms-win-core-heap-l1-1-0.dllがない」と表示され、インストールできない

HARUKA インストール時に「api-ms-win-crt-runtime-l1-1-0.dllがないためプログラムを開始できません。」（または「api-ms-win-core-heap-l1-1-0.dll」） と表示されてしまう場合、動作に必要なコンポーネントがパソコン内にインストールされていないことが考えられます。 下記対処を行っていただき、改善されるかご確認ください。

## 解決方法

### 1.WindowsUpdateを実施する

OSを最新に更新していただくことで、「**Visual Studio 2015 の Visual C++ 再頒布可能パッケージ**」がインストールされます。

:::success
Windows Update後、HARUKA を再度インストールしてください。
:::

### 2.「Visual Studio 2015 の Visual C++ 再頒布可能パッケージ」を再インストールする

Windows Updateを行っていただいても改善しない場合は、「**Visual Studio 2015 の Visual C++ 再頒布可能パッケージ**」を 一旦削除後、再インストールしていただき、HARUKA の動作を再度ご確認ください。

:::note 外部リンク
[Download Microsoft Visual C++ 2015 再頒布可能パッケージ Update 3 RC from Official Microsoft Download Center](https://www.microsoft.com/ja-jp/download/details.aspx?id=52685) 
:::

:::success
Microsoft のサイトより、「Visual Studio 2015 の Visual C++ 再頒布可能パッケージ」をダウンロードし、インストールします。
:::

### 3.改善しない場合

ご利用のパソコン環境で何らかの影響により「Visual Studio 2015 の Visual C++ 再頒布可能パッケージ」自体がインストールできない、 またはインストール完了後も改善しない場合、HARUKA のご利用に必要なコンポーネントがないため、ご使用いただくことができません。

:::success
別のパソコンをご用意いただき、HARUKA をご利用ください。
:::
