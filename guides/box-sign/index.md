---
rank: 225
category_id: box-sign
subcategory_id: null
is_index: true
id: box-sign
type: guide
total_steps: 4
sibling_id: guides
parent_id: guides
next_page_id: ''
previous_page_id: box-sign/cancel-sign-request
source_url: >-
  https://github.com/box/developer.box.com/blob/main/content/guides/box-sign/index.md
fullyTranslated: true
---
# Box Sign

署名リクエストの作成、リスト取得、再送信、キャンセルを実行するBox SignのAPIエンドポイントを使用することで、Box Signウェブアプリの全機能をプログラムによって利用できます。

## 有効化

<Message type="warning">

日本時間2021年7月27日に、Box Signをリリースしました。Business、Business Plus、Enterprise、Enterprise Suites、Starterの各プランにBox Signを追加する予定です。Box SignのAPIエンドポイントを使用するために管理者がBox Signを有効にする必要はありませんが、企業に導入する必要はあります。BoxインスタンスでBox Signが利用可能になる前に、管理者に通知されます。

</Message>

アカウントの種類でBox Signへのアクセスがサポートされている場合は、Box Sign APIを使用してリクエストを行うことができます。サポートされているタリフには、Business、Business Plus、Enterprise、Enterprise Suites、Enterprise Plus、Starterが含まれます。アカウントの種類を確認するには、\[**アカウント設定**] に移動し、\[**アカウント**] タブの \[**アカウントの詳細**] セクションまで下にスクロールします。管理者向けのアクセス制限の詳細については、[サポート記事][restrict]を参照してください。  

## 必須のスコープ

Box Signのエンドポイントを使用する前に、アプリケーションで以下の[スコープ][scopes]を有効にする必要があります。

* [Boxに格納されているすべてのファイルとフォルダの読み取り][read]
* [Boxに格納されているすべてのファイルとフォルダの書き込み][write]
* [署名リクエストの管理][sign]

<Message type="warning">

選択した認証方法や企業の設定によっては、新たに選択したスコープを使用する前に、アプリケーションで管理者の承認または再承認が必要になる場合があります。

</Message>

## レート制限

詳細については、[レート制限ガイド][ratelimit]を参照してください。

## テスト

機能が同等であるため、APIを利用する前に、[Boxウェブアプリを使用してBox Signの機能][webapp]をよく理解しておくと役に立つかもしれません。すべてのAPIエンドポイントと同様に、実稼働環境のコンテンツに影響を及ぼすリスクを取り除くため、[開発者サンドボックス環境][sandbox]でテストすることをお勧めします。

[scopes]: g://api-calls/permissions-and-errors/scopes

[read]: g://api-calls/permissions-and-errors/scopes/#read-all-files-and-folders

[write]: g://api-calls/permissions-and-errors/scopes/#read-and-write-all-files-and-folders

[sign]: g://api-calls/permissions-and-errors/scopes/#manage-signature-requests

<!-- i18n-enable localize-links -->

[restrict]: https://support.box.com/hc/en-us/articles/4404076971155-Enabling-Box-Sign

<!-- i18n-disable localize-links -->

[ratelimit]: g://api-calls/permissions-and-errors/rate-limits/#per-api-rate-limits

<!-- i18n-enable localize-links -->

[webapp]: https://support.box.com/hc/en-us/articles/4404105810195-Sending-a-document-for-signature

[sandbox]: https://support.box.com/hc/ja/articles/360043697274-Box管理者による開発者サンドボックスの管理

<!-- i18n-disable localize-links -->