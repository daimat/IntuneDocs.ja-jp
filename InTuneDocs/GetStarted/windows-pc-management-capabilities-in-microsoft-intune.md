---
title: "Intune PC ソフトウェア クライアントの機能 | Microsoft Intune"
description: "Intune ソフトウェア クライアントで Windows PC を管理する場合の Intune の機能について説明します。"
keywords: 
author: robstackmsft
manager: angrobe
ms.date: 08/25/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 77fa5c66-a87c-47df-964c-800eea509b33
ms.reviewer: owenyen
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: 12d75bc67fd61a2e807eed2543f21b756a65a900
ms.openlocfilehash: 3066ef98c0a1df6fc0ae455860635e7c12f82c4f


---

# Intune ソフトウェア クライアントを使用する場合の Windows PC の管理機能
ほとんどのシナリオでは、デバイスを Microsoft Intune に登録します。そうすることで、さらに多くの機能を使用できるようになります。 ただし、PC の管理には、Intune ソフトウェアを使用することもできます。このソフトウェアでは、次の機能が利用できます。

-   **ソフトウェア更新プログラムの管理。**PC を最新の状態に保ち、更新プログラムを適用する時間を決定できます。

-   **Windows ファイアウォールのポリシー。**この機能により、会社で使用する PC に、非アクティブまたは適切でない構成の Windows ファイアウォールが存在しないようにします。

-   **マルウェア対策。**Intune には、マルウェアから PC を保護するのに役立つ Endpoint Protection が含まれています。

-   **リモート アシスタンス。**ユーザーは Intune を使用して、IT サポート スタッフに連絡できます。IT サポート スタッフは、Intune に含まれているリモート デスクトップ機能を使用してサポートを提供できます (TeamViewer ソフトウェアが必要)。

-   **ソフトウェア ライセンス管理。**使用可能なソフトウェア ライセンスの数と、そのうちの使用中のライセンスの数を追跡します。
-   **アプリの展開。**管理対象の PC にソフトウェアを展開します。 ソフトウェア クライアントを使用して PC を管理する場合、一部のアプリ管理機能は利用できません。


Intune は、最大 7,000 台の Windows デバイスへのソフトウェア クライアントのインストールをサポートしています。

## オペレーティング システムの要件
Intune では、次の Windows バージョンを実行する PC を管理できます (32 ビットと 64 ビットの両方)。


-   **Windows Vista** - Business、Enterprise、および Ultimate バージョン

-   **Windows 7** - Pro、Enterprise、および Ultimate バージョン (Service Pack なし、または SP1)

-   **Windows 8** - Pro および Enterprise バージョン

-   **Windows 8.1** - Pro および Enterprise バージョン

- **Windows 10** - Pro、Education、および Enterprise バージョン


## ハードウェアに最低限必要な条件
Intune ソフトウェア クライアントのインストールの最小ハードウェア要件を次に示します。

|要件|説明|
|---------------|--------------------|
|Network (ネットワーク)|クライアントでは、PC がインターネット接続できる必要があります。|
|プロセッサとメモリ|PC のオペレーティング システムに対するプロセッサ要件と RAM 要件を参照してください。|
|ディスク領域|クライアント ソフトウェアをインストールする前に、200 MB の空きディスク領域が必要です。|

## その他の要件
Intune ソフトウェア クライアントのインストールの最小ソフトウェア要件を次に示します。

|要件|説明|
|---------------|--------------------|
|管理者のアクセス許可|クライアント ソフトウェアをインストールするアカウントは、その PC のローカル管理者のアクセス許可を持っている必要があります。|
|Windows インストーラー 3.1|PC には Windows インストーラー 3.1 以降がインストールされている必要があります。|
|互換性のないクライアント ソフトウェアを削除する|Intune PC クライアント ソフトウェアをインストールする前に、その PC から次のクライアント ソフトウェアをアンインストールする必要があります。<br /><br />-   Configuration Manager のすべてのバージョン<br />-   Microsoft Systems Management Server (SMS) のすべてのバージョン|

### 関連項目
[Microsoft Intune の登録済みデバイス管理機能](./mobile-device-management-capabilities-in-microsoft-intune.md)



<!--HONumber=Aug16_HO4-->


