---
title: "ユーザーとデバイスを編成するグループを作成する | Microsoft Intune"
description: "Intune サブスクリプションのユーザーとグループを作成する方法について説明します"
keywords: 
author: barlanmsft
manager: angrobe
ms.date: 08/29/2016
ms.topic: get-started-article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 5fdf98c8-fe67-4d7a-9837-ed1234348014
ms.reviewer: jeffgilb
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: 0c1e08cc49d75303f6793894e3c8a040f6e7a8b1
ms.openlocfilehash: 3b2f896ea6c3e66924dbd8b35fcddcccd0b65ca6


---


# ユーザーとデバイスを編成するグループを作成する
Intune の [グループ] を使用すると、デバイスとユーザーを柔軟に管理できます。 グループは、組織ごとのニーズ (地理的位置、部門、ハードウェアの特性など) に合わせて設定できます。一連のユーザーに対するポリシーの展開から、一連のデバイスに対するアプリケーションの展開まで、まざまな管理タスクをそれらのグループを使って実行することができます。

デバイスとユーザー グループは両方とも Intune 管理コンソールの [グループ] ワークスペースで作成します。

![管理コンソールの [グループ] ワークスペース](./media/groups.png)


> [!TIP]
> グループの使用方法の詳細については、「[Microsoft Intune でユーザーとデバイスの管理にグループを使用する](/intune/deploy-use/use-groups-to-manage-users-and-devices-with-microsoft-intune)」をご覧ください。


## デバイス グループを作成する
デバイス グループは、アプリや更新プログラムの展開のほか、各種機能の構成に使用します。 たとえば、"My Devices" というグループを設定するには、次の手順に従います。

1.  [Intune 管理コンソール](https://manage.microsoft.com/)で、**[グループ]** > **[概要]** > **[グループの作成]** を選択します。

2.  **[グループ名]** に「My Devices」と入力し、親グループ一覧から、**[すべてのデバイス]** を選択して、**[次へ]** を選択します。

3.  **[メンバーシップの基準の定義]** ページで、 **[すべてのデバイス]** を選択して、グループにモバイル デバイスとコンピューターの両方が含まれることを示します。

4.  **[ダイレクト メンバーシップの定義]** ページで、**[次へ]** をクリックします。 以前作成したグループに一部のデバイスが含まれていなかった場合、ここでデバイスを指定して、新しいグループに追加することができます。

5.  **[概要]** ページで、実行する操作を確認し、**[完了]** を選択します。

新しく作成したグループは、**[グループ]** 一覧の **[グループ]** ワークスペースにある **[すべてのデバイス]** の下に表示されます。 ここから、グループを編集または削除することもできます。

## ユーザー グループを作成する
ソフトウェアやデバイスのポリシーは、ユーザー グループを使用して展開します。 たとえば、"Intune Users" というグループを設定するには、次の手順に従います。

1.  [Intune 管理コンソール](https://manage.microsoft.com/)で、**[グループ]** > **[概要]** > **[グループの作成]** を選択します。

2.  **[グループ名]** に「Intune Users」と入力し、親グループ一覧から、**[すべてのユーザー]** を選択して、**[次へ]** を選択します。

3.  **[メンバーシップの基準の定義]** ページで、 **[グループのメンバーシップ]** を **[親グループのすべてのユーザー]**に設定します。

4.  **[メンバーを除外するセキュリティ グループ]** の横の **[参照]** を選択し、**[Company Administrator]** を選択します。 この除外設定により、Company Administrator アカウント (またはテナント管理者) に影響することなく、Intune Users グループを管理できます。

5.  **[ダイレクト メンバーシップの定義]** ページで、**[次へ]** をクリックします。 ここでは何も操作する必要はありません。Company Administrator を除いて、Intune Users グループにすべてのユーザーを含めるからです。

6.  **[概要]** ページで、実行する操作を確認し、**[完了]** を選択します。

新しく作成したグループは、**[グループ]** 一覧の **[グループ]** ワークスペースにある **[すべてのユーザー]** の下に表示されます。 ここから、グループを編集または削除することもできます。



### 次のステップ
これで終了です。 *Intune のクイック スタート ガイド*の手順 5 が完了しました。

>[!div class="step-by-step"]

>[&larr;**Intune のライセンスを管理する**](.\start-with-a-paid-subscription-to-microsoft-intune-step-4.md)       [**ポリシーとアプリを作成する**&rarr;](.\start-with-a-paid-subscription-to-microsoft-intune-step-6.md)  



<!--HONumber=Aug16_HO5-->


