---
title: 記錄CRM同步錯誤，以輕鬆進行疑難排解
description: 瞭解如何使用CRM同步處理錯誤的記錄來調查CRM同步處理問題，並讓它持續順暢地執行。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00.000Z
jira: KT-13875
thumbnail: KT-13875.jpeg
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
  - id: c68cd75e-5bca-4bc3-a60e-9e183f816441
    internal-label: Experience Manager Cloud Manager
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 749b293ab38b8ea5a5f72517bd5c3455399137c2
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%
---
# 記錄CRM同步錯誤以進行疑難排解

身為[!DNL Marketo Engage]管理員，檢查執行個體是否與CRM同步應該是您[每日常式](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}的關鍵部分。 雖然[通知區段](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} （在[!DNL Marketo Engage]介面的右上角找到）是您開始尋找和調查經常同步問題的地方，但有一個專業秘訣可幫助您以有條理的方式管理執行個體的健康狀況。[!DNL Adobe] Marketo Champion (2019-2022)，Amy Goldfine建議管理員使用者保留CRM同步錯誤的記錄，以便更輕鬆進行疑難排解。

![同步處理錯誤索引標籤的熒幕擷圖](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## 為什麼要保留CRM同步處理錯誤的記錄？

透過記錄CRM同步處理錯誤，[!DNL Marketo Engage]管理員可以與CRM管理員檢閱問題和趨勢，以修正根本原因。 請依照下列步驟，記錄您執行個體的CRM同步問題。

## 如何保留CRM同步處理錯誤的記錄

開始之前，請先下載[CRM同步錯誤記錄檔範本](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx)。

**步驟1：**&#x200B;移至[!DNL Marketo Engage]中的&#x200B;*[!UICONTROL 管理員]區段*。 在「*[!UICONTROL 整合]*」下，根據您使用的[!DNL CRM]，按一下「*[!DNL Salesforce]*」、「*[!DNL Microsoft Dynamics]*」或「*[!DNL Veeva]*」，然後按一下「*[!UICONTROL 同步錯誤]*」索引標籤。

**步驟2：**&#x200B;您可以透過[!UICONTROL 篩選器]面板](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}，選擇將錯誤的記錄[匯出為 [!DNL CSV] 檔案。 如果您只有幾個小時，直接從&#x200B;*[!UICONTROL 同步處理錯誤]*&#x200B;索引標籤複製並貼上會是很好的方法。

**步驟3：**&#x200B;記下發生錯誤的日期。

**步驟4：**&#x200B;輸入受該錯誤影響的人員記錄數目。 (有時您的CRM只會擲回一個人的錯誤。 有時會有許多人同時發生相同錯誤。)

**步驟5：**&#x200B;記下受錯誤影響之個人的電子郵件地址。 這可讓您輕鬆參考並與CRM管理員討論錯誤。

**步驟6：**&#x200B;將連結貼到該人員的[!DNL Marketo Engage]和[!UICONTROL CRM銷售機會/連絡人]記錄中的人員記錄。

**步驟7：**&#x200B;在最後一欄，貼上錯誤的實際文字。

## 接下來呢？

**識別錯誤碼：**&#x200B;若要瞭解錯誤碼，請查閱開發人員檔案[回應層級錯誤碼表格](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"}中的說明，並尋找解決錯誤的典型後續步驟。

## 作者

**Amy Goldfine**\
[!DNL Adobe]Marketo冠軍(2019-2022)
*創始人， MarketingOpsAdvice.com*

![Amy Goldfine](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**趙子楣**
*在[!DNL Adobe]*&#x200B;的採用與保留行銷經理

![趙子楣](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
