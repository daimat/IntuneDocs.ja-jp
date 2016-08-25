---
title: "デバイス グループのマッピングを使用してデバイスを分類する | Microsoft Intune"
description: "Microsoft Intune のデバイス グループ マッピングを使用して、ユーザー定義のカテゴリにデバイスをグループ化することで、それらのデバイスの管理が容易になります。"
keywords: 
author: robstackmsft
manager: angrobe
ms.date: 07/11/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 8b8c06a3-6b6c-4cf1-8646-b24fa9b1a39e
ms.reviewer: sumitp
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: 6716a3d1fb53dc3de0189f637d5664d0a2023d05
ms.openlocfilehash: 3eda87026f46ed911c83b874f7ef9362f0705492


---

# Microsoft Intune でデバイス グループのマッピングを使用してデバイスを分類する
Microsoft Intune の**デバイス グループ マッピング**を使用して、ユーザー定義のカテゴリにデバイスをグループ化することで、それらのデバイスの管理が容易になります。 

デバイス グループ マッピングでは、次のワークフローを使用します。
1. 使用するカテゴリごとに、Intune のデバイス グループを作成します。
2. デバイス グループ マッピング ルールを構成し、作成したデバイス グループに選択したカテゴリを対応付けます。
3. デバイスを登録するエンドユーザーは、構成されているカテゴリのうちのいずれかを選択する必要があります。 エンドユーザーがカテゴリを選択すると、デバイスは自動的に対応するデバイス グループに追加されます。
4. ポリシーやアプリを展開するときに、これらのデバイス グループを使用できるようになります。

カテゴリの例としては、次のものがあります。
* 個人用
* 販売時点管理デバイス
* デモンストレーション デバイス
* 営業
* アカウンティング
* Manager

必要に応じて、どのようなカテゴリでも構成することができます。

## デバイス グループ マッピングの構成方法
1. 使用するデバイス カテゴリごとに、Intune のデバイス グループを作成します。 グループの作成方法については、「[Microsoft Intune でユーザーとデバイスの管理にグループを使用する](use-groups-to-manage-users-and-devices-with-microsoft-intune.md)」を参照してください。
2. [Microsoft Intune 管理コンソール](https://manage.microsoft.com)で、**[管理者]** を選択します。
3. **[管理]** ワークスペースで、**[モバイル デバイス管理]** を展開してから、**[デバイス グループ マッピング]** を選択します。
4. **[デバイス グループ マッピング]** ページで、デバイス グループ マッピングを有効にします。
5. **[追加]** を選択し、新しいマッピング ルールを作成します。
6. **[デバイス グループ マッピング ルールの追加]** ダイアログ ボックスで、作成するカテゴリの名前を入力し、このカテゴリをマップするデバイスのコレクションをドロップダウン リストから選択します。 選択が完了したら、**[追加]** を選択します。
7. カテゴリとグループの追加が完了したら、**[保存]** を選択します。

これで、デバイスを登録するユーザーに対して、構成したカテゴリの一覧が表示されます。 ユーザーがカテゴリを選択して登録を完了すると、選択したカテゴリに対応するデバイス グループにデバイスが追加されます。

### 関連項目
[Microsoft Intune でユーザーとデバイスの管理にグループを使用する](use-groups-to-manage-users-and-devices-with-microsoft-intune.md)


<!--HONumber=Jul16_HO4-->

