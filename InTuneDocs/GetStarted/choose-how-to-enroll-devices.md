---
title: "モバイル デバイスの登録方法の選択 | Microsoft Intune"
description: "いくつかの簡単な質問に答えることによって、Intune でモバイル デバイスを登録する方法を決定する"
keywords: 
author: NathBarn
manager: angrobe
ms.date: 07/25/2016
ms.topic: article
ms.prod: 
ms.service: 
ms.technology: 
ms.assetid: cac62b64-3f8b-47ae-aa66-970c7ba15466
ms.reviewer: dagerrit
translationtype: Human Translation
ms.sourcegitcommit: c671610b9c56d8b92d126d9902cce9c8c689ed63
ms.openlocfilehash: aac4eee56ec7326b2ce466d19b580aa5f1388aea


---

# モバイル デバイスの登録方法の選択

次の質問に答えることで、管理するデバイスの最適な登録方法が決まります。

## **社員が自分のデバイスを持ち込みますか。それとも、会社が提供しますか。**

  - **ユーザー所有デバイス** - "Bring your own device" (BYOD) 登録
  - **会社所有デバイス** - COD 登録

> [!div class="button"]
[BYOD 登録 >](#what-byod-devices-can-your-users-enroll)   [COD 登録 >](#are-your-company-owned-devices-shared-or-do-they-have-dedicated-users)

## **ユーザーはどのような BYOD デバイスを登録できますか。**

> [!div class="button"]
[Android](/intune/deploy-use/set-up-android-management-with-microsoft-intune) [iOS と Mac](/intune/deploy-use/set-up-ios-and-mac-management-with-microsoft-intune) [Windows 10 Mobile と Window Phone](/intune/deploy-use/set-up-windows-phone-management-with-microsoft-intune) [Windows PC](/intune/deploy-use/set-up-windows-device-management-with-microsoft-intune)

## **会社所有デバイスを共有しますか。デバイスごとに専用の利用者が登録されますか。**

> [!div class="button"]
[共有 >](#what-operating-system-are-your-shared-devices-running)   [専用 >](#how-will-you-manage-dedicated-ios-devices)


## **共有デバイスが実行しているのはどのようなオペレーティング システムですか。**

  > [!div class="button"]
  [Windows >](/intune/deploy-use/enroll-corporate-owned-devices-with-the-device-enrollment-manager-in-microsoft-intune) [Android >](/intune/deploy-use/enroll-corporate-owned-devices-with-the-device-enrollment-manager-in-microsoft-intune) [iOS >](#how-will-you-manage-shared-ios-devices)

## **共有 iOS デバイスはどのような方法で管理しますか。**

  > [!div class="button"]
  [iOS の DEP 登録 >](/intune/deploy-use/ios-device-enrollment-program-in-microsoft-intune) [iOS の直接登録 >](/intune/deploy-use/ios-direct-enrollment-in-microsoft-intune)  [DEM 登録 >](/intune/deploy-use/enroll-corporate-owned-devices-with-the-device-enrollment-manager-in-microsoft-intune)

  - **Apple のデバイス登録プログラム (DEP)** - DEP で購入し、管理している iOS デバイスが対象となります。登録プロファイルが利用されます。 利用者がデバイスの電源を初めて入れると、デバイスが DEP プロファイルをダウンロードし、プロファイル DEP で登録します。

  - **Mac の Apple Configurator** - Apple Configurator は Mac PC で実行される Apple アプリケーションです。 USB ケーブルで iOS デバイスを Mac に接続し、デバイスに登録プロファイルをインストールできます。 デバイスを工場出荷時にリセットして登録できる場合、セットアップ アシスタント登録を使用します。 デバイスを工場出荷時にリセットしない場合、直接登録を使用します。

  - **デバイス登録マネージャー** - Intune のデバイス登録マネージャー (DEM) を使用して、管理者は 1 つのユーザー アカウントに多数のモバイル デバイスを登録できます。 これらのデバイスは、ユーザー アフィニティ (つまり専用ユーザー) を持つことはできず、ポータル サイト アプリをインストールしてサインインすることで登録する必要があります。

## **専用 iOS デバイスはどのような方法で管理しますか。**

  > [!div class="button"]
  [IMEI を持つタグ >](/intune/deploy-use/specify-corporate-owned-devices-with-international-mobile-equipment-identity-imei-numbers) [iOS DEP](/intune/deploy-use/ios-device-enrollment-program-in-microsoft-intune) [iOS 設定アシスタント](/intune/deploy-use/ios-setup-assistant-enrollment-in-microsoft-intune) [IMEI を持つタグ](/intune/deploy-use/specify-corporate-owned-devices-with-international-mobile-equipment-identity-imei-numbers)

  次のようにして、会社が所有するデバイスを専用ユーザーに登録できます。

  - **Apple のデバイス登録プログラム (DEP)** - DEP で購入し、管理している iOS デバイスが対象となります。登録プロファイルが利用されます。 利用者がデバイスの電源を初めて入れると、デバイスは DEP プロファイルをダウンロードして、Intune に登録します。

  - **Mac の Apple Configurator** - Apple Configurator は Mac PC で実行される Apple アプリケーションです。 USB ケーブルで iOS デバイスを Mac に接続し、デバイスに登録プロファイルをインストールできます。 デバイスを工場出荷時にリセットして登録できる場合、セットアップ アシスタント登録を使用します。

  - **IMEI 番号でのタグ付け** - 会社所有デバイスの IMEI (携帯機器の国際的な識別番号) をインポートすることで、Intune でデバイスに会社所有のタグを付けることができます。 その後、ポータル サイトをインストールし、デバイスを個人デバイスとして登録し、電子メール、アプリ、データなど、会社のリソースにアクセスできます。



<!--HONumber=Aug16_HO1-->


