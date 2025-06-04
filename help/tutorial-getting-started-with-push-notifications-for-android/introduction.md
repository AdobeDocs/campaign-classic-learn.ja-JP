---
title: Android 向けプッシュ通知の概要 - はじめに
description: このチュートリアルでは、Adobe Campaign からプッシュ通知を送信し、Android アプリでこれらの通知を受信する手順について説明します。
feature: Push
jira: KT-5951
doc-type: article
activity: setup
team: TM
role: Admin, Developer
level: Experienced
recommendations: noDisplay
exl-id: 291c2e3a-c126-439d-9753-06a4091bbda0
source-git-commit: b56c0af81ed73fa06fe4846d0794167d35a26305
workflow-type: ht
source-wordcount: '355'
ht-degree: 100%

---

# Android 向けプッシュ通知の概要 - はじめに

Adobe Campaign では、パーソナライズおよびセグメント化された [!DNL push] 通知を [!DNL iOS] および [!DNL Android] モバイルデバイスに送信できます。このチュートリアルでは、Adobe Campaign から [!DNL Android] アプリに [!DNL push] 通知を送信する手順を説明します。

## 前提条件

始める前に、次のものが必要です。

1) **Android モバイルアプリケーション**

   このチュートリアルでは、モバイルアプリケーションの設定に必要な詳細手順については説明しません。 [!DNL Campaign SDK] が統合された **[!DNL Android]モバイルアプリケーションが必要です**。

   必要な手順の詳細については、製品ドキュメントを参照してください。

   [Campaign SDK をモバイルアプリケーションに統合する](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-push-notifications/integrating-campaign-sdk-into-the-mobile-application.html?lang=ja)

   Experience Platform Mobile SDK も使用できます。 詳しくは、チュートリアルビデオを参照してください。

   [Experience Platform Mobile SDK を使用したプッシュチャネルの設定](https://experienceleague.adobe.com/docs/campaign-classic-learn/tutorials/sending-messages/push-channel/configure-push-using-aep-mobile-sdk.html?lang=ja)

2) インストール済みの **[!DNL Mobile App channel]パッケージ**

   [!DNL Mobile App channel] パッケージを [!DNL Campaign] インスタンスにインストールする必要があります。 次のビデオでは、[!DNL Mobile App channel] がインスタンスにインストールされているかどうかを確認する方法と、インストールしていない場合は、インストールの方法を説明します。

>[!VIDEO](https://video.tv.adobe.com/v/326544?quality=12&learn=on){transcript=true}

## チュートリアルの概要

[!DNL Neotrip] [!DNL Android] モバイルアプリのサブスクリプションを購入したお客様に、パーソナライズされたプロモーション[!DNL push]通知を送信したいと考えています。 [!DNL Neotrip] アプリには [!DNL Campaign SDK] が設定されていて、[!DNL Mobile App channel] が [!DNL Campaign] インスタンスでアクティブ化されています。

次の設定手順が必要です。

### ステップ 1：アプリの購読スキーマを拡張して[!DNL push]通知をパーソナライズする

[!DNL push] 通知をパーソナライズするには、まず[アプリ購読スキーマ](/help/tutorial-getting-started-with-push-notifications-for-android/extending-the-app-subscription-schema.md)を拡張し、ユーザーがサービスを購読する際にアプリから受け取るパーソナライズの値を格納できるようにします。

### ステップ 2：Campaign で Android サービスを設定してモバイルアプリケーションを作成する

次に、[Campaign で Android サービスを設定してモバイルアプリを作成する](/help/tutorial-getting-started-with-push-notifications-for-android/configuring-an-android-service-in-campaign.md)必要があります。このステップでは、[!DNL Neotrip] アプリをプッシュ通知のターゲットとして定義します。

### ステップ 3：プッシュ通知を設定および送信する

これで、[プッシュ通知を設定して送信する](/help/tutorial-getting-started-with-push-notifications-for-android/configuring-and-sending-push-notifications.md)準備が整いました。

## チュートリアルの開始

ステップ 1：[アプリ購読スキーマを拡張する](/help/tutorial-getting-started-with-push-notifications-for-android/extending-the-app-subscription-schema.md)
