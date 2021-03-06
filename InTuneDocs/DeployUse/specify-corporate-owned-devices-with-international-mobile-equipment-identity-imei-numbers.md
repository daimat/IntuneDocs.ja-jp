---
title: "IMEI 番号を指定する | Microsoft Intune"
description: "Microsoft Intune では、管理者は、モバイル デバイス プラットフォームの IMEI 番号をインポートして会社所有のモバイル デバイスを識別できます"
keywords: 
author: NathBarn
manager: angrobe
ms.date: 07/25/2016
ms.topic: article
ms.prod: 
ms.service: microsoft-intune
ms.technology: 
ms.assetid: 1712bd39-562b-4409-9cec-155d5f4d8a39
ms.reviewer: dagerrit
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: e9cbf5858cc4e860b540f421b6d463b8e7a429cf
ms.openlocfilehash: 4e2092182dbda4523c19afeabc34aa0166962c40


---

# IMEI (国際移動体装置識別番号) を使って企業所有のデバイスを指定する
Microsoft Intune では、管理者が IMEI (International Mobile Equipment Identity: 国際移動体装置識別番号) をモバイル デバイスのプラットフォームにインポートできます。IMEI 番号は、企業所有のモバイル デバイスを識別するために役立ちます。 Intune に登録すると、インポートされた IMEI 番号を持つデバイスを、**[グループ]**  >  **[概要]**  >  **[すべてのデバイス]** で確認できます。 **[デバイス グループ]** の一覧で、インポートされた IMEI 番号を持つデバイスは、**[所有権]** 欄に **[会社]** と表示されます。

1. [Microsoft Intune の管理コンソール](http://manage.microsoft.com)で、**[グループ]** &gt; **[すべてのデバイス]** &gt; **[会社の事前登録済みデバイス]** &gt; **[IMEI (すべてのプラットフォーム) を使用]** に移動し、**[デバイスの追加]** を選択します。 デバイスの追加方法は 2 つあります。

    -   **シリアル番号が含まれている CSV ファイルをアップロード** – csv ファイル 1 つあたりデバイス 5000 個または 5 MB を上限とする、2 つの列を持つヘッダーなしのコンマ区切り値のリスト (.csv) を作成します。

        |||
        |-|-|
        |&lt;IMEI 1&gt;|&lt;デバイス 1 の詳細&gt;|
        |&lt;IMEI 2&gt;|&lt;デバイス 2 の詳細&gt;|
        この .csv ファイルをテキスト エディターで開くと、次のように表示されます。

        ```
        AABBBBBBCCCCCCD,PO 1234
        AABBBBBBCCCCCCE,PO 1234
        ```

    -   **デバイスの詳細を手動で追加** - 最大 5 台のデバイスの IMEI 番号とデバイスの詳細を入力します。

   *詳細*は、管理作業で使う情報で、デバイスに関連付けられた IMEI 番号を識別できます。 この情報はデバイスには送信されませんが、Intune のコンソールに表示されます。

2.   **[次へ]** を選択します。
3.  **[デバイスの確認]** ウィンドウで、インポートされたデバイスの IMEI 番号を確認できます。 また、再インポートされている IMEI 番号の**詳細**を上書きするかどうかを決めることもできます。 **[上書き]** チェック ボックスをオフにすると、現在の詳細が保持されます。 **[完了]** を選択して、IMEI 番号をインポートします。
4.  追加した IMEI 番号および説明が、**[IMEI (すべてのプラットフォーム) を使用]** の一覧に追加されます。

IMEI 番号を持つデバイスを登録する (通常は、ユーザーがポータル サイト アプリをインストールし、登録プロセスを完了する) と、そのデバイスは会社所有としてタグ付けされ、**IMEI デバイス** グループに登録されたデバイスとして表示されます。



<!--HONumber=Jul16_HO4-->


