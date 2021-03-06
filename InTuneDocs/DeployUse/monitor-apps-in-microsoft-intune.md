---
title: "アプリの展開を監視する | Microsoft Intune"
description: "Intune を使用して展開したアプリを監視する方法について説明します。"
keywords: 
author: robstackmsft
manager: angrobe
ms.date: 07/13/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 5daad56d-71c8-455b-8a55-f8b33e279a8a
ms.reviewer: mghadial
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: d3412150f96f81937b6ea471d4a27ac42da875f8
ms.openlocfilehash: a0fd24b430cce49cf7d3ba395341ed07912b9404


---


# Microsoft Intune でアプリの展開を監視する

## アプリの展開を監視する
Intune 管理コンソールで管理対象アプリの展開の状態を確認できます。

### 管理するアプリとその状態を確認するには
**[アプリ]** ワークスペースで、**[アプリ]** ノードを選択し、**[アプリ]** を選択します。

管理しているアプリの一覧が表示されます。 コンソール ウィンドウの下のウィンドウでアプリを選択すると、インストール状態が表示されます。 さらに詳細を表示するには、この状態を選択します。 たとえば、状態に **[1 人のユーザーがこのソフトウェアを利用しています]** と表示されている場合、そのメッセージを選択すると、ユーザーの名前を確認できます。

> [!TIP]
> **[フィルター]** ドロップダウン リストを利用すると、インストールできなかったアプリや正常に展開されたアプリなど、指定した基準に一致するアプリのみを表示できます。
>
> ![アプリ フィルターの例](./media/app-filters.png)

また、**[ダッシュボード]** ワークスペースには、アプリの状態の概要が表示されます。 概要内のどこでもよいのでクリックすると、アプリの一覧が表示されます。

## アプリに関する詳細を表示するには
アプリの一覧で、アプリを選択し、**[プロパティの表示]** を選択します。

アプリの **[ソフトウェア プロパティ]** ページで、次のいずれかのタブを選択します。**[全般]** - アプリとそのインストール状態に関する一般的な情報が表示されます。**[デバイス]** - アプリの対象となる展開が正常にインストールされているデバイスが表示されます。**[ユーザー]** - アプリの対象となる展開が正常にインストールされているデバイスのユーザーが表示されます。

前述のように、**[フィルター]** ドロップダウン リストを利用し、各タブに表示される値を構成できます。



<!--HONumber=Aug16_HO2-->


