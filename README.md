# CryptoPiTouch NEMTUSHackathon

![wordlogo](images/wordlogo.png)

CryptoPiTouch for NEMTUSハッカソン2024提出用リポジトリ

## 概要

NFC を活用したクリプトタッチ決済システムです。  
本システムは、決済情報を受け渡すための端末機器と、端末機器と通信するモバイルアプリで構成されています。

### 端末機器

【これから書く】

### モバイルアプリ

【これから書く】

## アプリ配布

今回のハッカソン提出では Android のみの配布となります。(成果物提出時点)

[CryptoPiTouch Beta (arm64-v8a)](https://tgvrock.github.io/CryptoPiTouch_NEMTUSHackathon/apps/crypto-pi-touch-beta.apk)

古い機種の場合、アプリが起動しないことがあります。
以下のアプリもお試しください。

[CryptoPiTouch Beta (armeabi-v7a)](apps/crypto-pi-touch-beta-armeabi-v7a.apk)  
[CryptoPiTouch Beta (x86_64)](apps/crypto-pi-touch-beta-x86_64.apk)

iOS でも動作することは確認しておりますので、将来的には App Store / Google Play での配信を目標にしております。

## 使い方

【これから書く】

## デモ動画

容量が大きいため、Wi-Fi環境での視聴推奨です。

### [Symbol](demos/demo_symbol.mp4)

### [Ethereum](demos/demo_ethereum.mp4)

### [Astar](demos/demo_astar.mp4)

## 連絡先

感想、質問、不具合情報、なんでも大歓迎です！

- X (旧Twitter)
  - [まめしば](https://twitter.com/maromaro1989)
  - [だーりんピ](https://twitter.com/darling_pi_)

## トラブルシュート

- タッチ後 MetaMask は開くが、署名ダイアログが表示されない

## TODO

以下の挙動・事象は現状未対応ですが、将来的に対応したいと思います。

### 未実装項目

- 連携先の署名アプリ・ウォレットアプリで署名キャンセルされた場合の動作
  - 本アプリに戻った後、読み込み完了ダイアログが表示されたままとなり、再試行もキャンセルもできません。
  - ホーム画面に戻ることでリセットできます。
- Metamask で、決済するチェーン以外が選択されていた場合の動作
  - Metamask 側でネットワーク変更されますが、その後は署名キャンセル同様の動作になります。

### 現在判明している不具合や未実装項目

- [iOS] アプリ起動後、初回の端末設定が必ず失敗します。
  - 二回目以降は大丈夫です。

### 改善したいこと

- 取引価格をリアルタイム更新できるようにする。
  - 現在は店舗側ページが開いた時・受取アドレスを変更した時のみ更新される。
- 通知 (承認になった時、着金時、EVM系全般)
- 店舗側ページ : EVMチェーンのQR読み取り対応
- 店舗側ページ : EVMチェーンの受取履歴
