---
description: メニューに「HARUKA に転送」が出てこない
sidebar_position: 5
---

# HARUKAに転送が無い

## Illustrator の場合

HARUKA インストール時に、Illustrator プラグインがインストールできなかった可能性があります。また、Illustrator をバージョンアップをした際は、新たにインストールする必要があります。

:::success
Illustrator を閉じてから、プラグインインストーラーを実行してください。
:::

![スタートメニューの HARUKA の中にある「Illustratorプラグインインストール」を実行します。](/assets/20191101_01.png)

![または、C:\\\Program Files (x86)\\\HARUKA の中にある「AiPluginSetup.exe」を実行します。](/assets/20191101_02.png)

### 手動インストールの手順

・プラグインファイルの場所（コピーしてください）

Program Files (x86)\HARUKA\Ai\20.0

・インストールする場所（ペーストしてください）

Program Files\Adobe\Adobe Illustrator CC 2019\Presets\ja_JP\スクリプト

上記フォルダにコピーしたファイルを置きます。

## CorelDRAW の場合（2019以前）

HARUKA インストール時に、CorelDRAW プラグインがインストールできなかった可能性があります。

:::success
CorelDRAW を閉じてから、プラグインインストーラーを実行してください。
:::

![スタートメニューの HARUKA の中にある「CorelDRAWプラグインインストール」を実行します。](/assets/20191101_03.png)

![または、C:\\\Program Files (x86)\\\HARUKA の中にある「CorelPluginSetup.exe」を実行します。](/assets/20191101_04.png)

### 手動インストールの手順（2019以前）

・プラグインファイルの場所（コピーしてください）

Program Files (x86)\HARUKA\Corel\20.0

・インストールする場所（ペーストしてください）

Users\（ユーザー名）\AppData（隠しフォルダ）\Roaming\Corel\CorelDRAW Graphics Suite X8\Draw\GMS

上記フォルダにコピーしたファイルを置きます。

### 手動インストールの手順（2020以降）

・プラグインファイルの場所（コピーしてください）

C:\Users\ユーザー名\AppData\Local\HARUKA\Corel\20.0

・インストールする場所（ペーストしてください）

Users\（ユーザー名）\AppData（隠しフォルダ）\Roaming\Corel\CorelDRAW Graphics Suite X8\Draw\GMS

上記フォルダにコピーしたファイルを置きます。



### HARUKA のアイコン**が**無い（2019以前）

:::success
CorelDRAW メニューのマクロマネージャーから HARUKA プラグインを実行してください。
:::

CorelDRAW を起動して、新規ドキュメントを作成します。

![「ツール > マクロ > マクロマネージャー」をクリックします。](/assets/20191101_05.png)

適当なパスを作成、選択して HARUKA に転送します。

![マクロマネージャーの「OhLaserHARUKA > OhLaser > HARUKA_Plugin」をダブルクリック](/assets/20191101_06.png)

すると、HARUKA の青いアイコンが出てきます。

![ドラッグして上のツールバーに入れてください。](/assets/20191101_07.png)

### HARUKA のアイコンが他に変わってしまった場合（CorelDRAW）

ツール > オプションウインドウを開きます。

![カスタマイズ > コマンド > ファイル > マクロをクリック](/assets/20191101_08.png)

![OhLaser.HARUKA_Plugin を選択して、外観タブの参照ボタンをクリック](/assets/20191101_09.png)

HARUKA アイコンを選択します。

![C:\\\Users\\\ユーザー名\\\AppData\\\Local\\\HARUKA\\\Corel\\\20.0の中にあるHアイコンを選択します。](/assets/20191101_10.png)

:::success
アイコンを変更したら、ツールバーのアイコンを確認してください。
:::



### HARUKA のアイコン**が**無い（2020以降）

:::success
CorelDRAW メニューのカスタマイズから HARUKA アイコンを作成してください。
:::

CorelDRAW を起動して、新規ドキュメントを作成します。

![「ツール > オプション> カスタマイズ」をクリックします。](</assets/image(12).png>)

![「コマンド > ドロップダウン> マクロ」をクリックします。](</assets/image(15).png>)

![「Ohlaser.HARUKA_Plugin」をツールバーへドラックアンドドロップし「OK」](</assets/image(17).png>)

:::success
アイコンがデフォルトのままの場合は「参照」よりHARUKAマークを設定してください。

Users\（ユーザー名）\AppData（隠しフォルダ）\Roaming\Corel\CorelDRAW Graphics Suite X8\Draw\GMS
:::

![](</assets/image(18).png>)

ツールバーにプラグインが表示され、オブジェクトを選択しアイコンをクリックするとHARUKAに転送されます。
