---
title: "Windows エディションのアップグレード ポリシー設定 | Microsoft Intune"
description: "Intune を使用して Windows 10 デバイスを最新バージョンに自動的にアップグレードする方法について説明します。"
keywords: 
author: robstackmsft
manager: angrobe
ms.date: 08/29/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 8589866a-3f13-489b-a5cd-cee017d16d54
ms.reviewer: jeffgilb
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: 06a9c78300d7ff384299957102114c69c43a1ad5
ms.openlocfilehash: 45130e3e12968d9df579a7a9d0cade0343b7c165


---

# Microsoft Intune のエディションのアップグレード ポリシー設定
Microsoft Intune の**エディションのアップグレード ポリシー**を使用して、次に挙げる Windows 10 のバージョンのいずれかを実行するデバイスを自動的に新しいエディションにアップグレードできます。
* [Windows] 10 Desktop
* Windows 10 Holographic
* [Windows] 10 Mobile

## アップグレードを開始する前に
デバイスを最新バージョンにアップグレードし始める前に、次のいずれかを用意する必要があります。
* ポリシーで対象とするすべてのデバイスに新しいバージョンの Windows をインストールするための有効なプロダクト キー (Windows 10 Desktop エディションの場合)。 マルチ ライセンス認証キー (MAK) またはキー マネジメント サーバー (KMS) キーのどちらかを使用できます。
**または、**ポリシーで対象とするすべてのデバイスに新しいバージョンの Windows をインストールするためのライセンス情報を含む、Microsoft からのライセンス ファイル (Windows 10 Mobile エディションと Windows 10 Holographic エディションの場合)。
* 対象とする Windows 10 デバイスが Microsoft Intune に登録されている必要があります。 エディションのアップグレード ポリシーは、Intune PC クライアント ソフトウェアを実行する PC で使用できません。

## エディションのアップグレード ポリシー設定

|設定の名前|説明|
|-|-|
|**名前**|エディションのアップグレード ポリシーの名前を入力します。|
|**説明**|必要に応じて、Intune コンソールでの識別に役立つポリシーの説明を入力します。
|**アップグレード後のエディション**|対象とするデバイスのアップグレード後の Windows 10 Desktop、Windows 10 Holographic、または Windows 10 Mobile のバージョンをドロップダウン リストから選びます。
|**プロダクト キー**|Microsoft から取得した、対象とするすべての Windows 10 デスクトップ デバイスをアップグレードするために使用できるプロダクト キーを指定します。<br>プロダクト キーを含むポリシーを作成した後でプロダクト キーを編集することはできません。 これは、セキュリティ上の理由からキーが隠されるためです。 プロダクト キーを変更するには、キー全体を再入力する必要があります。
|**ライセンス ファイル**|**[参照]** を選択し、Microsoft から取得した、対象とするデバイスのアップグレード後の Windows Holographic、または Windows 10 Mobile エディション用のライセンス情報を含むライセンス ファイルを選択します。

### 関連項目
[Microsoft Intune ポリシーを使用してデバイスの設定と機能を管理する](manage-settings-and-features-on-your-devices-with-microsoft-intune-policies.md)



<!--HONumber=Aug16_HO5-->


