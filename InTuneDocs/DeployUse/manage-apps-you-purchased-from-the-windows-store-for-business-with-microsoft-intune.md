---
title: "ビジネス向け Windows ストアのアプリの管理 | Microsoft Intune"
description: "Intune コンソールからボリューム購入したアプリを管理および展開する場合に、Microsoft Intune をビジネス向け Windows ストアに接続する"
keywords: 
author: robstackmsft
manager: angrobe
ms.date: 07/13/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 8e38d47d-0c5e-40ce-b379-29d3657f5c28
ms.reviewer: jeffgilb
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: d40ec3b5b7c5c4ee2cfd48a95ada0dadcaa80be4
ms.openlocfilehash: 077029a962797a18fab27c3f1f5340eae6edfe04


---

# ビジネス向け Windows ストアから購入したアプリを Microsoft Intune で管理する
[ビジネス向け Windows ストア](https://www.microsoft.com/business-store)では、組織用のアプリを見つけて、個別または大量購入することができます。 Microsoft Intune にストアを接続することで、Intune コンソールから大量購入アプリを管理することができます。 たとえば、
* ストアから購入したアプリの一覧を Intune に同期することができます。
* 同期されているアプリは Intune 管理コンソールに表示され、他のアプリと同様に展開することができます。
* 使用可能なライセンス数、および Intune 管理コンソールで使用中のライセンス数を追跡することができます。
* 使用可能なライセンス数が不足している場合、Intune はアプリの展開とインストールをブロックします。

## アップグレードを開始する前に
ビジネス向け Windows ストアからアプリを同期して展開する前に、以下のことを確認してください。
* 組織のモバイル デバイス管理機関として Intune を構成する必要があります。 詳細については、「[Microsoft Intune にデバイスを登録する準備](get-ready-to-enroll-devices-in-microsoft-intune.md)」を参照してください。
* ビジネス向け Windows ストアのアカウントにサインアップする必要があります。
* Intune に Windows ビジネス ストア アカウントを関連付けた後で別のアカウントに変更することはできません。
* Intune に対して、ストアから購入したアプリを手動で追加したり、削除したりすることはできません。 ビジネス向け Windows ストアとの同期のみが可能です。
* Intune は、ビジネス向け Windows ストアから購入したオンライン ライセンスされたアプリのみを同期します。
* この機能を使用するには、デバイスが Active Directory ドメイン サービスまたはワークプレースに参加している必要があります。
* 登録デバイスは、1511 リリースの Windows 10 を使用している必要があります。

## Intune にビジネス向け Windows ストア アカウントを関連付ける
Intune コンソールで同期を有効にする前に、以下の手順に従って、Intune を管理ツールとして使用するようにストア アカウントを構成する必要があります。
1. Intune へのサインインに使用したものと同じテナント アカウントを使用して、ビジネス ストアにサインインしていることを確認します。
2. ビジネス ストアで、**[設定]** > **[管理ツール]** の順に選択します。
3. [管理ツール] ページで、**[管理ツールの追加]** を選択し、**[Microsoft Intune]** を選択します。

これで、作業を続行し、Intune コンソールで同期を設定することができます。

## 同期を構成する

1. [Microsoft Intune 管理コンソール](https://manage.microsoft.com)で、**[管理者]** を選択します。
2. **[管理]** ワークスペースで、**[モバイル デバイス管理]** を展開し、**[ビジネス向けストア]** を選択します。
3. **[ビジネス向け Windows ストア]** ページで、以下の操作を行います。
 * ビジネス向け Windows ストアにまだサインアップしていない場合は、サインアップ用のリンクをクリックしてサインアップを行います。
 * サインアップしたら、**[同期の構成]** を選択します。
4. **[ビジネス向け Windows ストア アプリの同期の構成]** ダイアログ ボックスで、**[ビジネス向け Windows ストアの同期を有効にする]** を選択します。
5. **[言語]** ドロップダウン リストで、Intune コンソールで表示するビジネス向け Windows ストアのアプリに使用する言語を選択します。 アプリは、どの言語を使用して表示するかに関係なく、使用可能なエンド ユーザーの言語でインストールされます。
6. **[OK]** をクリックします。

## アプリを同期する

1. **[ビジネス向け Windows ストア]** ページで、**[今すぐ同期]** を選択し、ストアから購入したアプリと Intune を同期します。
2. **[アプリ]** ワークスペースで、**[管理されているソフトウェア]** > **[ライセンス供与されているソフトウェア]** の順に選択し、使用可能なアプリを表示し、購入したアプリが正しくインポートされたことを確認します。 このノードのアプリは、所有しているライセンスの合計数と、使用可能なライセンスの数と共に表示されます。

## アプリの展開

他の Intune アプリを展開する場合と同じように、ストアからアプリを展開します。 詳細については、「[Deploy apps in Microsoft Intune](deploy-apps-in-microsoft-intune.md)」 (Microsoft Intune でアプリを展開する) を参照してください。
ビジネス向け Windows ストア アプリを展開すると、アプリをインストールする各ユーザーによってライセンスが使用されます。 展開されたアプリに対して使用可能なライセンスをすべて使用すると、それ以上コピーを展開することはできません。 以下のいずれかの操作を実行する必要があります。
* 一部のデバイスからアプリをアンインストールする。
* 現在の展開の範囲を絞り、十分なライセンスがあるユーザーのみを対象にする。
* ビジネス向け Windows ストアからアプリのコピーをさらに購入する。

> [!Important]
> 展開されたアプリは、最初にデバイスを登録したユーザーのみが利用できます。 他のユーザーは、そのアプリにアクセスすることができません。


### 関連項目
[Microsoft Intune でモバイル デバイスのアプリを追加する](add-apps-for-mobile-devices-in-microsoft-intune.md)



<!--HONumber=Aug16_HO1-->


