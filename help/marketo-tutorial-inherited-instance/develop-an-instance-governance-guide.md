---
title: 使用檔案開發執行個體治理指南
description: 瞭解如何建立強大的程式，以建立和維護您的檔案和變更記錄檔 [!DNL Marketo Engage] 執行個體。 這不僅可節省團隊分享知識的時間，也可提升執行個體的健全度和效率。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-14103
thumbnail: KT-14103.jpeg
hide: false
exl-id: e127b84d-ef92-4527-a0e6-a36af35b7ee0
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 1%

---

# 使用檔案開發執行個體治理指南

當您步入舊版[！DNL [!DNL Marketo Engage]]例如，它經常會面臨缺乏最新功能與技術檔案的挑戰。 身為管理員，建立准則以確保適當的執行個體治理是您不可忽視的核心責任。 這是重要策略之一， [在既定的環境中工作時提高效率 [!DNL Marketo Engage] 例項](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582).

此逐步教學課程源自[！DNL [!DNL Adobe] Marketo Champion] (2018)的Nick Hajdin將引導您完成此程式，以概要說明您的執行個體設定、記錄您的主要營運方案並維護 [!DNL changelog] 以強制實行嚴格的治理政策。

## 為何要為繼承的執行個體開發執行個體治理指南和檔案？

詳細檔案和 [!DNL changelog] 對於[！DNL]中的有效管理和知識傳授至關重要 [!DNL Marketo Engage]]執行個體。 持續追蹤您在執行個體設定期間所做的變更和決定，有助於您：

1. 以可擴充的方式更輕鬆地訓練內部使用者。
2. 在[！DNL中更有效率地建置 [!DNL Marketo Engage]]長期而言。
3. 繼續維持執行個體的健康與衛生，讓您不必花費數小時探索電子郵件， [稽核軌跡](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html)、和 [活動記錄](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html) 以取得內容。
4. 節省傳輸[！DNL的時間 [!DNL Marketo Engage]新增知識[！DNL [!DNL Marketo Engage]]管理員（如果您的團隊遇到任何變動）。

## [！DNL [!DNL Marketo Engage]]治理指南101

治理指南是執行個體設定和系統設計要求的真實來源。 建議納入本檔案的重要資訊包括：

* 方案/資料夾結構
* 使用者和角色許可權
* 通訊限制
* 治理標準
* 授與使用者對平台的存取權之前的內部使用者訓練

## 如何為您的[！DNL]開發及維護治理指南 [!DNL Marketo Engage]]例項

### 步驟1：識別您目前的治理指南和檔案狀態

* **我找不到任何繼承執行個體的檔案：** 如果您最近啟動了一個新角色，但找不到繼承執行個體的任何檔案， **前往步驟2** 並開始使用我們提供的可下載範本。
* **我有檔案檔案：** 恭喜，這是個好兆頭！ 請務必檢閱其相關性，以檢視上次進行變更的時間。 如果您的團隊成員未主動維護更新，建議您重新整理，並教育內部使用者如何使其保持最新狀態。

### 步驟2：識別要包含在[！DNL]中的元素 [!DNL Marketo Engage]]檔案與 [!DNL Changelogs]

格式因雲端型平台和共用檔案而異。 您可以設計符合組織需求的格式。 [以下是簡單的檔案和變更記錄檔Excel範本](/help/marketo-tutorial-inherited-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx)說明您可以開始使用的重要元素。 這些類別包括：

* 文件
   * 計畫範本名稱
   * Channel
   * 建立日期
   * 建立者
   * 計畫的目的
   * 狀態
   * 方案範本的連結
   * 注意
* Changelog
   * 計畫範本名稱
   * 變更日期
   * 更新者
   * 更新的目的
   * 變更前的體驗（包含連結/熒幕擷取畫面）
   * 變更後的體驗（包含連結/熒幕擷取畫面）
   * 方案的URL

### 步驟3：識別並記錄主要作業程式的目前狀態

首先，找出在訂閱層級具有影響的主要作業方案。 範例包括資料管理 [!DNL Campaign]s，銷售機會生命週期，銷售機會評分， [!DNL CRM] 同步和傳遞能力。

對於每個已識別的作業方案，記錄其目前狀態。 其中包括有關方案目的、設定、相關智慧行銷活動，以及與其他工具整合（如果適用）的詳細資訊。

### 步驟4：強制 [!DNL Changelog] 維護

下一步是為您的[！DNL]建立嚴格的治理政策 [!DNL Marketo Engage]]執行個體強制執行&quot;[!DNL Changelog] 維護作業。」 此原則可確保完整記錄整個執行處理中對作業程式所做的任何更新。

教育您的團隊這些檔案的重要性，以及如何正確存取和更新它們。 指派維護變更記錄的責任可能會有所幫助，因此一些指定的行銷作業團隊成員或管理員會一致地記錄變更並提供簽章。

### 步驟5：集中處理檔案

建立中央位置或存放庫，以儲存與您的[！DNL]相關的所有檔案 [!DNL Marketo Engage]]執行個體。 這可以是共用磁碟機、專用資料夾或雲端系統。

### 步驟6：定期檢閱和更新

排程定期審查您的檔案，以確保它保持準確和最新。 在繁忙的時刻很容易被忽略。 主動設定行事曆上的提醒，以確保您的團隊定期進行更新，以反映作業程式中的任何變更或最佳化。

## 接下來還有什麼?

開始下載此專案 [簡單範本](/help/marketo-tutorial-inherited-instance/_assets/downloads/[!DNL Adobe]_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx)。

請依照上述步驟開發您的治理指南和檔案。 處理此程式時，請謹記下列經驗法則：

**更新您現有的檔案：**
讓您的檔案保持在最新狀態非常重要。 如果在過去3年內未修改檔案，請預留時間在稽核執行個體時修訂檔案。

**共用與訓練：**
分享您的檔案和 [!DNL changelog] 與相關團隊成員討論，並教導他們如何更新這些記錄。

**定期檢閱：** 在一年當中預先安排時間進行檢閱與維護，以包含任何新變更、最佳化或調整。

維護您全面且最新的檔案 [!DNL Marketo Engage] 執行個體可節省您長期的時間和精力，並有助於有效管理執行個體。

### 作者

**尼克·哈伊丁**
[！DNL [!DNL Adobe] Marketo達人] (2018)
*[!DNL Digital Technology Senior Manager at Accenture]*

![尼克·哈伊丁](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**趙藹明**
*採用與保留行銷經理，[!DNL Adobe]*

![趙藹明](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
