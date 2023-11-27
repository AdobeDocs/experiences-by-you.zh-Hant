---
title: 記錄CRM同步錯誤，以輕鬆進行疑難排解
description: 瞭解如何使用CRM同步處理錯誤的記錄來調查CRM同步處理問題，並讓它持續順暢地執行。
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 記錄CRM同步錯誤，以輕鬆進行疑難排解

作為 [!DNL Marketo Engage] 管理員，檢查執行個體是否與CRM同步應該是您的一項關鍵工作， [每日常式](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (請在您的右上角找到 [!DNL Marketo Engage] 介面)可協助您開始尋找及調查經常發生的同步問題，這裡提供專業秘訣，可協助您以有條理的方式管理執行個體健康情況。 [!DNL Adobe] Marketo Champion (2019-2022)，Amy Goldfine建議管理員使用者保留CRM同步錯誤的記錄，以便更輕鬆進行疑難排解。

![[同步錯誤]索引標籤的熒幕擷圖](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## 為什麼要保留CRM同步處理錯誤的記錄？

透過記錄CRM同步錯誤， [!DNL Marketo Engage] 管理員可以與CRM管理員檢閱問題和趨勢，以修正根本原因。 請依照下列步驟，記錄您執行個體的CRM同步問題。

## 如何保留CRM同步處理錯誤的記錄

開始之前，請先下載 [CRM同步錯誤記錄範本](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**步驟1：** 前往 *[!UICONTROL 管理員] 區段* 在 [!DNL Marketo Engage]. 在 *[!UICONTROL 整合]*，按一下 *[!DNL Salesforce]*， *[!DNL Microsoft Dynamics]*，或 *[!DNL Veeva]*，視何者而定 [!DNL CRM] 您使用，然後 *[!UICONTROL 同步錯誤]* 標籤。

**步驟2：** 您可以選擇 [將錯誤記錄匯出為 [!DNL CSV] 檔案透過 [!UICONTROL 篩選] 面板](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. 如果您只有幾個小時，請直接從 *[!UICONTROL 同步錯誤]* 按Tab鍵即可。

**步驟3：** 記下發生錯誤的日期。

**步驟4：** 輸入受該錯誤影響的人員記錄數。 (有時您的CRM只會擲回一個人的錯誤。 有時會有許多人同時發生相同錯誤。)

**步驟5：** 記下受錯誤影響之個人的電子郵件地址。 這可讓您輕鬆參考並與CRM管理員討論錯誤。

**步驟6：** 在[！DNL]中貼上個人記錄的連結 [!DNL Marketo Engage]]和 [!UICONTROL CRM銷售機會/連絡人] 該人員的記錄。

**步驟7：** 在最後一欄，貼上錯誤的實際文字。

## 接下來還有什麼?

**識別錯誤代碼：** 若要瞭解錯誤代碼，請檢視開發人員檔案中的說明 [回應層級錯誤代碼表格](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} 並尋找解決錯誤的典型後續步驟。

## 作者

**艾米·戈德芬**\
[!DNL Adobe] Marketo達人(2019-2022)
*創始人， MarketingOpsAdvice.com*

![艾米·戈德芬](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**趙藹明**
*採用與保留行銷經理，位於[!DNL Adobe]*

![趙藹明](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
