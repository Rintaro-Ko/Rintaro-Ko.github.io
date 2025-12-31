# MyTeslaWearApp Support Site

このリポジトリは、Tesla用非公式ウォッチアプリ **MyTeslaWearApp** のための静的ファイルをホストしています。
GitHub Pagesを利用して、Tesla APIの認証フローやドメイン所有権確認に必要なファイルを提供します。

## 主なコンテンツ

### 1. OAuth Callback (`/callback`)
Teslaアカウント認証後のリダイレクト先ページです。
AndroidアプリがDeep Link (`https://rintaro-ko.github.io/github.io/callback`) を捕捉できなかった場合、このページが表示され、Javascriptおよび手動ボタンによってアプリへの復帰（Intent呼び出し）を試みます。

- **URL:** `https://rintaro-ko.github.io/github.io/callback`
- **ファイル:** `callback/index.html`

### 2. Tesla Fleet API 公開鍵
Tesla Fleet APIとの通信（Command Signingなど）に必要な公開鍵をホストしています。

- **URL:** `https://rintaro-ko.github.io/.well-known/appspecific/com.tesla.3p.public-key.pem`