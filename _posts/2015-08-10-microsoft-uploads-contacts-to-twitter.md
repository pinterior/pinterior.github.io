---
layout: posts
title: MicrosoftがメールアドレスをTwitterにアップロードする話
tags: microsoft windows windows-phone
---


Twitterにはスマートフォン用アプリ等からアップロードされたアドレスを確認できる[Contacts Dashboard](https://twitter.com/settings/contacts_dashboard)というページが存在します。
ここに2人の知人のメールアドレスがなぜか出現したため、何が原因なのか調べることにしました。

最初は使用しているWindows 8タブレットやWindows Phoneがアップロード元ではないかと疑っていましたが、それらの利用を止め、Twitterからアップロードされたメールアドレスを削除しても、どこからかアップロードされて再出現するという状況が続きました。消去法でOutlook.comに預けている連絡先がMicrosoftのサーバから自動的にアップロードされているのではないかという疑いが強くなったため、以下の手順で確認を行いました。

* 新規にMicrosoftアカウントを取得する
   * ポピュラーな姓と名の組み合わせから生成したアドレスを300件ほどインポートする
* 新規にTwitterアカウントを取得する
   * チュートリアルに従って60ユーザーほどフォローする
* people.live.comでTwitterとの連携を設定する

![Connect Twitter](/images/live-com-connect-twitter.png)

連携を設定して12時間ほど経過すると、Twitterにメールアドレスがアップロードされていました。
(“We only share what you've asked us to share, and nothing else.”と書いてあったのに…)

名前が全員“No name”であること、また300件中15件ほどアップロードされてそれ以上アップロードされる様子はないことなど、正常な動作ではなさそうなのでそのうち直るとよいですね。

Outlook.com(Windows Live, Hotmail)のユーザはもちろん、Windows(8以降)やWindows Phoneのユーザもこのふるまいに注意してください。一部の機能は利用できなくなりますが、Twitterの[Applications](https://twitter.com/settings/applications)のページからMicrosoftの各種サービスへのアクセス許可をすべて取り消せばアップロードは止まると思います。

![Contacts Dashboard](/images/twitter-com-contacts-dashboard.png)
