---
title: 原生CRM聯結器的同步欄位
description: 瞭解如何策略性地選取要供Marketo Engage使用的基本CRM欄位，以簡化您的初始CRM整合。 進行資料字典練習，找出您需要的欄位，以順利進行CRM同步作業，協助銷售與行銷團隊維持一致。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04T00:00:00Z
jira: KT-14811
thumbnail: KT-14811.jpeg
source-git-commit: 47ab8875bc4e41595cd40550330e43a88357b68d
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---


# 原生CRM聯結器的同步欄位

您在組織內使用Salesforce或Microsoft Dynamics嗎？ 若是如此，您可以使用Marketo Engage的原生CRM聯結器(即Salesforce、Microsoft Dynamics和Veeva)，透過在Marketo Engage和CRM之間無縫共用相關資訊，協調行銷和銷售活動。 在設定初始CRM同步之前，請務必識別您要在兩個系統之間同步的欄位，以保持您的Marketo Engage資料庫整潔。

進一步瞭解如何使用Adobe Professional Services建議的最佳實務進行此練習。 請跟隨瞭解標準欄位和自訂欄位，並記錄它們在Marketo Engage與您的CRM之間的關係。

## 在整合您的CRM與Marketo Engage之前，識別要同步的欄位

將CRM與Marketo Engage整合時，您可能不需要同步處理所有CRM欄位以進行Marketo Engage。 對您所需的欄位採取策略性態度，有助於您的Marketo Engage執行個體更有效率地處理資料流程。

您的Marketo Engage與CRM系統之間的初始同步會自動關聯大部分的現有標準欄位（即電子郵件、名字/姓氏、公司等）。 此外，聯結器也會同步 [自訂欄位](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} 針對「銷售機會」、「聯絡人」、「帳戶」和「商機」，方法是在自動對應至您CRM中這些欄位的Marketo Engage中建立新欄位。

在執行初始同步之前，識別並組織您要從CRM同步的欄位，是原生聯結器設定流程中的關鍵步驟。 我們稱之為資料字典練習，可幫助您將建立的重複欄位數降到最低，並讓任何後續的重新對應步驟儘可能順暢地進行。 此練習通常包含行銷和銷售團隊以及您的CRM管理員的輸入內容，以確保只有相關欄位才會同步至您的Marketo Engage執行個體。

## 如何建置您的資料字典

一般而言，最佳實務是僅同步行銷所需的CRM欄位。 從這項練習開始，以整理CRM中需要對應至Marketo Engage的欄位，並在第一次正確執行初始CRM同步。

>[!NOTE]
>如果您的CRM中有自訂欄位，在開始初始Marketo Engage前已有對應的自訂欄位，則會在Marketo Engage中為CRM欄位建立新的「重複」欄位。 您可以將CRM欄位重新對應到原始Marketo Engage欄位，並在初始同步完成後隱藏重複欄位，但您需要聯絡 [Adobe客戶支援](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} 以達成此目的。 如需詳細資訊，請參閱步驟7。

**步驟1：** 建立您CRM中目前可用欄位的粗略清單，並標示您是否要這些欄位以Marketo Engage顯示。

* 在決策程式中加入CRM管理員、行銷和銷售團隊的意見回饋。
* 記錄每個欄位的API名稱和欄位型別
* 決定這些欄位應該具有的存取Marketo Engage層級（即唯讀或讀寫）


**步驟2：** 檢閱 [「管理員>欄位管理」區段](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} Marketo Engage識別先前直接在系統中建立並要納入同步的任何自訂欄位。

* 記錄每個欄位的API名稱和欄位型別。
* 表示在您的CRM中已有相同欄位的欄位。
* 表示在您的CRM中沒有同等欄位的欄位。


**步驟3：** 開始使用預設對應欄位建置資料字典

* 由於Marketo Engage使用一般資料庫，因此建議您依照下列方式設定資料字典的格式：

   * 第一欄：Marketo Engage欄位名稱
   * 第二欄：Marketo EngageAPI名稱
   * 第三欄： [Marketo Engage欄位型別](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} （即布林值、貨幣、日期等）
   * 在後續欄中，針對CRM物件型別（銷售機會、連絡人、帳戶、機會）重複此步驟，並加入您希望Marketo Engage存取層級的額外欄（即讀取、寫入、編輯）
  <br>

  以下是它看起來像的範例：
  ![資料字典表格](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* 首先，新增將自動對應至CRM的預設欄位：

   * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
   * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
   * [Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* 確認Marketo Engage中的每個預設欄位都符合您CRM中要同步處理的欄位。 例如，Marketo Engage中的「已取消訂閱」欄位可能是您CRM中的「電子郵件選擇退出」欄位。
* 調整CRM API名稱、許可權和 [資料型別](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} 如有必要。

**步驟4：** 新增其他欄位至資料字典

* 包括顯示名稱、所需的CRM許可權和每個欄位的資料型別。
* 如果CRM中有欄位但沒有Marketo Engage，請以CRM欄位的相同值填入Marketo Engage顯示和API名稱。
* 如果Marketo Engage中有欄位但沒有CRM，請以所需的值填入CRM顯示名稱，但將CRM API名稱保留空白，直到建立欄位為止。
* 如果兩個系統中都存在相等的欄位，請將它們加入同一行，並指示它們需要在「資料字典」工作表最右側的「備註」區段中重新對應。

>[!NOTE]
>如果您打算建立同步篩選器欄位([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"})，請務必將其納入此步驟，但將API名稱保留空白，直到在您的CRM中建立欄位為止。

**步驟5：** 與您的CRM管理員一起檢閱資料字典

* 在CRM中為Marketo Engage中已存在的欄位建立欄位，並使用新CRM欄位的顯示和API名稱更新資料字典。
* 在您的CRM中的潛在客戶與聯絡人物件之間執行欄位對應([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"})。 當Lead轉換為Contact時，這可確保可將欄位合併為Marketo Engage的單一欄位。
* 請確定Marketo同步設定檔具有適當許可權，可存取資料字典中所述的每個欄位：
   * [在Salesforce中設定設定檔許可權](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"}
   * [在Microsoft Dynamics中設定設定檔許可權](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
   * [在Veeva中設定設定檔許可權](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}

**步驟6：** 執行初始同步

* 請確認您要與Marketo Engage同步的所有欄位，在CRM中都具有資料字典所定義的適當許可權。
* 確定所有欄位  ***非*** 與Marketo Engage同步的方式為 [在Marketo同步設定檔中隱藏](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. 在稍後新增欄位至同步處理會比移除無意同步處理的欄位容易得多。
* 您是否將CRM連線至「同步篩選器」欄位？ 如果您同步至Salesforce，請聯絡Adobe客戶支援，以確保篩選功能在開始初始同步處理前已開啟。


**步驟7：** 檢閱Marketo Engage中的「欄位管理」區段

* 確認/更新新同步欄位的顯示和API名稱。
* 識別任何可能需要重新對應的重複欄位。 重複欄位會在以下幾種情況下發生：
   * 如果Marketo Engage中已存在對等欄位，則CRM中的自訂欄位會在第一次同步時在Marketo Engage中建立新的（可能重複）欄位。
   * Marketo-Engage-Only自訂欄位(即直接在Marketo Engage中建立的欄位)可能會有從CRM同步的同等欄位。



**步驟8：** 如果出現重複的欄位，請聯絡Adobe客戶支援以執行重新對應

* 如需需要重新對應的欄位，請聯絡支援人員，並提供下列資訊：
   * CRM建立的新重複欄位的顯示和API名稱。
   * 顯示您希望CRM欄位對應到的Marketo Engage欄位名稱。
   * 請參考此範例 [此處](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}.
* 重新對應完成後，請檢閱Marketo Engage中重新對應欄位的API名稱，並更新資料字典的「API名稱」欄中的值，以確保其包含最準確的資訊。

## 接下來呢？

* 建立您的資料字典以整理CRM整合的欄位。
* 請熟悉CRM的初始同步程式

>[!BEGINTABS]

>[!TAB Salesforce]

瞭解Marketo Engage和Salesforce如何共同合作，讓您的銷售和行銷資料保持同步。

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**影片中使用的連結：**

* [瞭解Salesforce同步](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.html){target="_blank"}

* [將Marketo欄位新增至Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.html){target="_blank"}

* [在Salesforce中建立Marketo使用者(Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.html){target="_blank"}

* [連線Marketo和Salesforce(Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.html){target="_blank"}

* [使用者需要先在Salesforce端設定連線應用程式，才能繼續前往Marketo和Salesforce Sync。](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.html){target="_blank"}

* [Salesforce同步狀態](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status.html){target="_blank"}

* [隱藏和取消隱藏欄位](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field.html){target="_blank"}

* [教學課程：瞭解如何將Marketo同步至您的CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

瞭解Microsoft Dynamics 365同步如何運作，並正確設定設定，以允許兩個系統相互溝通。

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**影片中使用的連結：**

* [瞭解Microsoft Dynamics同步](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync.html){target="_blank"}

* [下載Marketo銷售機會管理解決方案](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution.html){target="_blank"}

* [更新適用於Microsoft Dynamics的Marketo解決方案](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.html){target="_blank"}

* [授予使用者端ID和應用程式註冊的同意](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration.html)

* [驗證Microsoft Dynamics同步](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync.html){target="_blank"}

* [同步狀態](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status.html){target="_blank"}

* [修正Dynamics驗證同步問題](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues.html){target="_blank"}

* [建立自訂Dynamics同步篩選器](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynmaics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [檢視組織服務URL](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url.html){target="_blank"}

* [在Dynamics中刪除欄位之前，請先編輯要同步的欄位](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics.html){target="_blank"}

* [教學課程：瞭解如何將Marketo同步至您的CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!ENDTABS]

### 作者

{{peter-livadas}}

{{amy-chiu}}