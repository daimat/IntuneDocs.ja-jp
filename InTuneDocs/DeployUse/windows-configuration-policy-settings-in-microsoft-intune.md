---
title: "Windows ポリシー設定 | Microsoft Intune"
description: "Intune の Windows 全般構成ポリシー (Windows 8.1 以降) を使用して、登録済みの Windows 8 および Windows 8.1 デバイスの設定を構成します。"
keywords: 
author: robstackmsft
manager: angrobe
ms.date: 07/19/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 6982a2bc-aafa-475a-9236-4840b709e5a1
ms.reviewer: jeffgilb
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: 7fdfe64a18fe359ee4b3b4507ef4108ad65ab573
ms.openlocfilehash: 3102e4637c61bbae002fb30947acd1f82204ac93


---

# Microsoft Intune の Windows ポリシー設定
Microsoft Intune の **Windows 全般構成ポリシー (Windows 8.1 以降)** を使用して、登録済みの Windows 8 および Windows 8.1 デバイスの以下の設定を構成します。

## 適用性の設定

|設定の名前|説明|
|----------------|----------------------------------|
|**Windows 10 にすべての構成を適用する**|Windows 8、および Windows 8.1 デバイスに加え、Windows 10 デバイスに、このポリシーの設定を適用できます。|

## セキュリティ設定

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**必要なパスワードの種類**|英数字や数値のみなど、必要なパスワードの種類を指定します。|[はい]|○|
|**必要なパスワードの種類 - 文字セットの最小数**|パスワードに含める必要がある文字セットの数を指定します。 文字セットには、小文字、大文字、数字、および記号の 4 種類があります。 ただし、iOS デバイスの場合は、この設定でパスワードに含める必要がある記号の数を指定します。|Yes|○|
|**パスワードの最小文字数**<sup>1</sup>|パスワードに必要な最小の長さ (文字数) を構成します。|Yes|○|
|**デバイスをワイプするまでの連続サインイン エラーの数**|サインインの試みがこの回数だけ失敗した場合は、デバイスがワイプされます。|[はい]|○|
|**画面がオフになるまでの非アクティブな時間 (分)**|デバイスのアイドル状態が許容される時間 (分) を指定します。この時間を超えると、ロックを解除するためにパスワードが必要となります。| [はい]|○|
|**パスワードの有効期限 (日数)**|デバイスのパスワードの変更が必要になるまでの日数を指定します。|○|○|
|**パスワードの履歴を記憶する**|過去に使用したパスワードをユーザーが構成できるかどうかを指定します。|○|○|
|**パスワードの履歴を保存する** - **前のパスワードを再利用できないようにする**|デバイスで記憶される、以前に使用したパスワードの数を指定します。|○|○|
|**ピクチャ パスワードと PIN を許可する**|ピクチャ パスワードと PIN を使用できるようにします。 ピクチャ パスワードが許可されている場合、ユーザーは画像に対するジェスチャーでサインインすることができます。 PIN が許可されている場合、ユーザーは 4 桁のコードを使用してすばやくサインインできます。|Yes|Yes|
<sup>1</sup>Windows RT を実行するデバイスにパスワードの長さポリシーを展開すると、ユーザーは、現在のパスワードがポリシー要件に準拠している場合でもパスワードを再設定するように求められます。

## 暗号化の設定

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**モバイル デバイスの暗号化を要求する**<sup>1</sup>|デバイス上のファイルを必ず暗号化するようにします。<br>Windows Phone 8 デバイスの場合、これを **[はい]**に設定する必要があります。|○|×|
<sup>1</sup> Windows 8.1 が実行されているデバイスの追加情報

-   Windows 8.1 が実行されているデバイスで暗号化を適用するには、 [Windows の 2014 年 12 月付け MDM クライアント更新プログラム](http://support.microsoft.com/kb/3013816) を各デバイスにインストールする必要があります。

-   Windows 8.1 デバイスに対してこの設定を有効にすると、デバイスのすべてのユーザーに Microsoft アカウントが必要になります。

-   暗号化を機能させるには、デバイスが Microsoft [InstantGo](http://blogs.windows.com/bloggingwindows/2014/06/19/instantgo-a-better-way-to-sleep/) ハードウェア認定要件を満たしている必要があります。

-   デバイスで暗号化を適用すると、回復キーは、ユーザーの Microsoft アカウントからしかアクセスできなくなります。また、OneDrive アカウントからアクセスする必要があります。 ユーザーの代わりにこのキーを回復することはできません。

## マルウェアの設定

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**ネットワーク ファイアウォールを必須にする**|Windows ファイアウォールを有効にすることを要求します。|Yes|×|
|**SmartScreen を有効にする**|Windows SmartScreen の使用を必須とします。|Yes|×|

## システムの設定

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**自動更新を必須にする**|デバイス上の自動更新設定を有効にします。|[はい]|×|
|**自動更新を必須にする – 自動的にインストールする更新プログラムの最低限の分類。**|自動的にインストールする更新プログラムの分類を選択します。<br /><br />-   **重要** – 重要として分類されたすべての更新プログラムをインストールします。<br />-   **推奨** – 重要または推奨として分類されたすべての更新プログラムをインストールします。|Yes|×|
|**ユーザー アカウント コントロール**|デバイス上のユーザー アカウント制御 (UAC) の使用を必須とします。|Yes|×|
|**診断データの送信を使用する**|デバイスが Microsoft に診断情報を送信できるようにします。|Yes|×|


## クラウドの設定 – ドキュメントおよびデータ

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**作業フォルダーの URL**|作業フォルダーの URL を設定して、デバイス間でドキュメントを同期できるようにします。|[はい]|×|

## 電子メールの設定

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**Windows メール アプリケーションで Microsoft アカウントをオプションにする**|Microsoft アカウントを使用せずに Windows メール アプリケーションにアクセスできるようにします。|Yes|×|

## アプリケーションの設定 - ブラウザー

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**オートコンプリートを使用する**|ユーザーがブラウザーのオートコンプリートの設定を変更できるようにします。|Yes|×|
|**ポップアップ ブロックを使用する**|ブラウザーのポップアップ ブロックを有効または無効にします。|○|×|
|**プラグインを使用する**|ユーザーが Internet Explorer にプラグインを追加できるようにします。|[はい]|×|
|**アクティブ スクリプティングを使用する**|ブラウザーで Active X スクリプトなどのスクリプトを実行できるようにします。|[はい]|×|
|**不正行為の警告を使用する**|詐欺目的の疑いがある Web サイトの警告を有効または無効にします。|Yes|×|
|**1 単語の入力でイントラネット サイトにアクセスできるようにする**|Bing など、1 つの単語を使用して Internet Explorer に移動先の Web サイトを指示できるようにします。|[はい]|×|
|**イントラネット ネットワークの自動検出を使用する**|Internet Explorer でイントラネット サイト用にセキュリティを構成できるようにします。|○|×|
|**インターネットのセキュリティ レベル**|インターネット サイトに使用する Internet Explorer のセキュリティ レベルを設定します。|[はい]|×|
|**イントラネットのセキュリティ レベル**|イントラネット サイトに使用する Internet Explorer のセキュリティ レベルを設定します。|[はい]|×|
|**信頼済みサイトのセキュリティ レベル**|信頼済みサイト ゾーンのセキュリティ レベルを構成します。|Yes|×|
|**制限付きサイトのセキュリティ レベル**|制限付きサイト ゾーンのセキュリティ レベルを構成します。|Yes|×|
|**Do Not Track ヘッダーを送信する**|Internet Explorer で、訪問したサイトに Do Not Track ヘッダーを送信します。|[はい]|×|
|**エンタープライズ モード メニューへのアクセスを許可する**|Internet Explorer からエンタープライズ モード メニュー オプションへのアクセスをユーザーに許可します。<br>この設定を選択した場合は、さらに **[ログ レポートの場所]** を指定できます。これは、エンタープライズ モード アクセスが有効にされた Web サイトの記録となるレポートの URL を表します。|Yes|×|
|**エンタープライズ モード サイト リストの場所**|エンタープライズ モードがアクティブな場合に、エンタープライズ モードを使用する Web サイトの一覧の場所を指定します。|Yes|×|

## デバイス機能の設定 - 移動体通信

|設定の名前|説明|Windows 8.1 および Windows RT 8.1|Windows RT|
|----------------|----------------------------------|--------------|
|**データ ローミングを許可する**|デバイスが移動体通信ネットワーク上にある場合はデータ ローミングを使用できるようにします。|Yes|×|



### 関連項目
[Microsoft Intune ポリシーを使用してデバイスの設定と機能を管理する](manage-settings-and-features-on-your-devices-with-microsoft-intune-policies.md)



<!--HONumber=Aug16_HO3-->

