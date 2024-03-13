# CryptoPiTouch NEMTUSHackathon

![wordlogo](images/wordlogo.png)

CryptoPiTouch for NEMTUSハッカソン2024提出用リポジトリ

## 概要

## アプリ

今回のハッカソン提出では Android のみの配布となります。(成果物提出時点)

[CryptoPiTouch Beta (arm64-v8a)](https://tgvrock.github.io/CryptoPiTouch_NEMTUSHackathon/apps/crypto-pi-touch-beta.apk)

古い機種の場合、アプリが起動しないことがあります。
以下のアプリもお試しください。

[CryptoPiTouch Beta (armeabi-v7a)](apps/crypto-pi-touch-beta-armeabi-v7a.apk)  
[CryptoPiTouch Beta (x86_64)](apps/crypto-pi-touch-beta-x86_64.apk)

iOS でも動作することは確認しておりますので、将来的には App Store / Goggle Play での配布を目標にしております。

## 使い方

準備中。。。

## デモ

### [Symbol](demos/demo_symbol.mp4)

### Ethereum【準備中。。。】

### Astar【準備中。。。】

## トラブルシュート

## 連絡先

- X (旧Twitter)
  - [だーりんピ](https://twitter.com/darling_pi_)
  - [まめしば](https://twitter.com/maromaro1989)

## TODO

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
- EVMチェーンのQR読み取り対応
- EVMチェーンの受取履歴
