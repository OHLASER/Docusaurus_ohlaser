---
sidebar_position: 1
description: パソコンが、HARUKA のシステム条件に合っているか確認
---

# 日々の清掃

# デプロイ
githubとの連携方法を確認しておりました。
npm run build で公開するファイルをビルドして、gh-pages ブランチにpushするという手順になります。

試したことはないのですが、原理的には、ビルドして作成されたファイルを、[https://docs.oh-laser.com/](https://docs.oh-laser.com/) にアップロードすれば、github を経由しなくても、ドキュメントサイトをサブドメインで公開できそうです。

イメージしておりますのは、githubで共同編集し、npm run build で必要な公開ファイルを作成し、ftpで docs.oh-laser.com の該当フォルダにアップロードする、という運用です。

### 静的ファイルの生成方法
まず、公式ドキュメントから、英語になりますが、以下のページの記載です。
[https://docusaurus.io/docs/deployment](https://docusaurus.io/docs/deployment)

> npm run build
> Once it finishes, the static files will be generated within the build directory.

上記は、「npm run build」を実行すると、build ディレクトリに静的なファイルが生成される、という意味です。
このbuildディレクトリのファイルを任意のサーバーにアップロードすれば動作します。

ただし、環境設定が必要です。
[https://docusaurus.io/docs/deployment#configuration](https://docusaurus.io/docs/deployment#configuration)
にあるように、
url と baseUrl の設定が必要です。

例えば、以下のように設定します。

url: '[http://timerec.colsystem.biz](http://timerec.colsystem.biz/)',
baseUrl: '/build/',

npm run build として、アップロードした結果は、以下にアップロードすることになります。

[http://timerec.colsystem.biz/build/](http://timerec.colsystem.biz/build/)

実際に、上記に初期設定のものを、FTPでアップロードしてみました。
ぜひアクセスしてみてください。（借り物のURLで申し訳ありません…）
[http://timerec.colsystem.biz/build/docs/hello](http://timerec.colsystem.biz/build/docs/hello)
もあります。

---

urlは、サーバー名を指定します。
そのため、「[https://timerec.colsystem.biz](https://timerec.colsystem.biz/)」のみで大丈夫です。
[https://docs.oh-laser.com/](https://docs.oh-laser.com/) なら、そのまま「[https://docs.oh-laser.com](https://docs.oh-laser.com/)」ですね。

baseURLは、設置するフォルダ名を書きます。
もし「[https://timerec.colsystem.biz/build/](https://timerec.colsystem.biz/build/)」なら、「/build/」だけ書きます。
[https://docs.oh-laser.com/](https://docs.oh-laser.com/) なら、そのまま「/」ですね。

url と baseUrl を並べると、ちょうどファイルをアップロードしたトップURLを形成するようにします。

[https://timerec.colsystem.biz](https://timerec.colsystem.biz/) + /build/ -> [https://timerec.colsystem.biz](https://timerec.colsystem.biz/) + /build/
[https://docs.oh-laser.com](https://docs.oh-laser.com/) + / -> [https://docs.oh-laser.com/](https://docs.oh-laser.com/)

docs/hello は、docusaurus の中のフォルダ、ファイル構成によって決まります。
よって、上記設定には含ませません。

上記は最初設定すれば、あとはほぼ変更することのない設定ですので、ご安心ください。

---

## 20220726_初稿
お待たせしたしました。docusaurusの初稿納品させていただきます。

- サイドバーについては、docフォルダの構造から自動生成するようにしております。ドキュメント自体はダミーですが、フォルダを作成し、その中の「_category_.json」を修正することで、カテゴリラベルの設定が可能です。
- サイト内検索については、オーブンになっているものでないと高度な検索の設定ができません。今はローカルでの検索機能を持ったプラグインを入れ、テスト可能としております。

具体的なドキュメントをコピーしてみて、さらに設定を詰めさせていただければと思います。ひとまず、今回のファイルをお試しください。

■　試験方法

添付のファイルを解凍してください。
ターミナルを開き、解凍したフォルダに移動してください。
「npm run serve」でテストサーバーが動作します。
ブラウザで「[http://localhost:3000/build/」にアクセスしてみてください](http://localhost:3000/build/%E3%80%8D%E3%81%AB%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B9%E3%81%97%E3%81%A6%E3%81%BF%E3%81%A6%E3%81%8F%E3%81%A0%E3%81%95%E3%81%84)。
