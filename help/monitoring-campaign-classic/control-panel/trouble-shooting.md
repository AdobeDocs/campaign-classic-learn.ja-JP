---
title: コントロールパネルのトラブルシューティング
description: コントロールパネルを使用すると、インスタンスおよび許可リストの IP アドレスごとに SFTP ストレージを監視および管理できます。
feature: Control Panel
jira: KT-2938
doc-type: article
activity: use
team: PM
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: fd6e6e36-54e4-4f1a-96fc-1a750e400d50
    internal-label: Campaign Classic v7
feature_v2:
  - id: ae9127b0-c11d-467b-903d-a84cef43f6ed
    internal-label: Control Panel
source-git-commit: d4d4654e5b2dee85947373b8dcf139754844b316
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 81%
---

# [!UICONTROL コントロールパネル]のトラブルシューティング

## ログインとホームページ

### 症状：Experience Cloud にログインできない

**対処方法：**
ユーザーは、自分の IMS 組織 ID（xxx）を見つける必要があります。 管理者は、管理するインスタンスごとに、ユーザーを製品プロファイル「Campaign-xxx-Admins」に追加する必要があります。 ユーザーがすべてのインスタンスの管理者であっても、自分自身をユーザーとして追加する必要があります。

### 症状：Experience Cloud ホームで、[!UICONTROL コントロールパネル]にアクセスするためのリンクがユーザーに表示されない

**原因：**
ユーザーは、製品プロファイル _Campaign-xxx-Administrators/Admin_&#x200B;にユーザーとして追加されるまで、リンクを表示しません。

**対処方法：**
管理者が、管理する各インスタンスの製品プロファイル _Campaign-xxx-Admins_ にユーザーを追加する必要があります。 ユーザーがすべてのインスタンスの管理者であっても、自分自身を「ユーザー」として追加する必要があります。

### 症状：インスタンスが [!UICONTROL コントロールパネル]に表示されない

**原因：**
見つからないインスタンスについて、最も可能性の高いユーザーを「ユーザー」製品プロファイル _Campaign-xxx-Administrators/Admin_&#x200B;として追加する必要があります

**対処方法：**
管理者が、管理する各インスタンスの製品プロファイル _Campaign-xxx-Admins_ にユーザーを追加する必要があります。 ユーザーがすべてのインスタンスの管理者であっても、自分自身を「ユーザー」として追加する必要があります。

### 役立つビデオ

>[!VIDEO](https://video.tv.adobe.com/v/35064?captions=jpn&quality=12&learn=on){transcript=true}

*IMS組織IDを確認（00:26分）*

>[!VIDEO](https://video.tv.adobe.com/v/35055?captions=jpn&quality=12&learn=on){transcript=true}

*製品プロファイル管理者に管理者を追加して、[!UICONTROL &#x200B; コントロールパネル &#x200B;] （01:03分）*&#x200B;を使用できるようにする方法

### 参考になるドキュメント

* [コントロールパネルの理解](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=ja)
* [[!UICONTROL コントロールパネル]に対する権限の管理](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=ja)

## SFTP サーバーへの接続の確立（クライアントまたは API）

SFTP サーバーに接続するには、以下が必要です。

* SFTP サーバーへの接続元となる IP アドレスを[!UICONTROL 許可リストに登録する]こと
* Adobe Campaign に登録する必要がある秘密キーと公開キーのペア
* SFTP サーバーに直接接続する場合は、SFTP クライアントソフトウェアが必要です

### 参考になるドキュメント {#helpful-docs}

* [SFTP サーバーへのログイン](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=ja)

