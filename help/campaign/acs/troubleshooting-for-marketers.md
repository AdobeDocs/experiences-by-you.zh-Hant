---
title: 行銷人員疑難排解
description: 瞭解最常見的錯誤，有助於更快速地解決問題，並提高生產力。 這些故障排除提示可幫助您有效地解決發生的類似錯誤。
solution: Campaign Standard
feature-set: Campaign
feature: Workflows
role: User
level: Beginner, Intermediate, Experienced
doc-type: Article
last-substantial-update: 2023-05-18T00:00:00Z
jira: KT-13256
thumbnail: KT-13256.jpeg
source-git-commit: a27a5538a7009d00d01227865ced4c5039147496
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 2%

---

# 行銷人員疑難排解：5個常見的工作流程與傳送錯誤

作者： [蘇拉傑帕特拉文](https://www.linkedin.com/in/suraj-p-51612053/){target="_blank"}，資深顧問， Meijer

身為資深工程師和客戶專家， [!DNL Adobe] Experience Cloud過去五年的產品，我啟用業務使用者於 [邁耶](https://www.meijer.com/){target="_blank"}成立於1934年的美國超級中心連鎖店，使用ACS執行複雜的行銷和交易式行銷活動。 我處理過的幾個專案包含自訂行銷活動，以儲存個人化的選件和訂單詳細資料，並整合 [!DNL Adobe] 區段擷取的Audience Manager和客戶分析。


在使用ACS期間，我遇到一些錯誤，解決這些錯誤會非常耗時且令人沮喪。 瞭解最常見的錯誤，有助於更快速地解決問題，並提高生產力。 以下是我的疑難排解提示，可協助您有效解決類似錯誤。

## 資料型別不符錯誤

**錯誤碼：**
`PGS-220000 PostgreSQL error: ERROR: operator does not exist: character varying = bigint`

**原因：**
當您嘗試使用不同資料型別的欄位進行調解時，這些型別的錯誤會出現在工作流程中。 例如，當您使用具有字串欄位的載入檔案上傳檔案，並嘗試協調字串欄位與資料型別為int的設定檔欄位時。

![data-type-mismatch-error](/help/_assets/kt-13256/data-type-mismatch.png)

**解決方案：**
將「載入檔案」活動中欄位的資料型別變更為您符合的欄位。 開啟「載入檔案」活動。 移至「COLUMN DEFINITION」標籤，並變更所需欄位的資料型別。


![data-type-mismatch-solution](/help/_assets/kt-13256/data-type-mismatch-solution.png)

## 傳遞個人化錯誤

**錯誤碼：**
`The schema for profiles specified in the transition ('') is not compatible with the schema defined in the delivery template ('nms:recipient'). They should be identical.`

**原因：**
當您傳送電子郵件至某個地址，但該電子郵件或任何其他識別碼並未與設定檔進行調解時，會出現此錯誤。 若要傳送電子郵件通訊，電子郵件或識別碼應一律連結至設定檔。

![具有調解活動的工作流程](/help/_assets/kt-13256/del-persn-error-wf.png)

**解決方案：**
具有收件者表格的載入檔案中必須有通用ID。 此公用索引鍵會將載入檔案聯結至調解活動中的收件者表格。 電子郵件不可傳送至收件者表格中不存在的記錄，而這需要在工作流程中進行此調解步驟。 這樣做時，您會使用設定檔中的電子郵件ID等識別碼，調解傳入的載入檔案活動。 此 `nms:recipient` 結構描述是指設定檔表格，並使用設定檔調解傳入記錄，以便在電子郵件準備期間使用。

請參閱調解活動的熒幕擷圖，如下所示。

![具有調節明細的工作流程](/help/_assets/kt-13256/del-persn-error-wf-solution.png)

進一步瞭解 [調解](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/data-management-activities/reconciliation.html?lang=en).

## 通用欄位資料集錯誤

**錯誤碼：**
`The document types of inbound events (''and'') are incompatible (step 'Exclusion'). Unable to perform the operation. `

**原因：**
此問題會在使用時發生 **排除活動** 在ACS工作流程中，當根據ID執行排除時，當主要集和排除集的欄位名稱不同時。


![通用欄位資料集錯誤](/help/_assets/kt-13256/dataset-error.png)

**解決方案：**

有兩種方式可解決此錯誤：

1. 在主要和排除中使用相同的欄位名稱，並將該欄位用作ID

   或

2. 使用JOINS排除方法，選取要排除記錄的欄位。

![通用欄位資料集錯誤 — 解決方案 ](/help/_assets/kt-13256/dataset-error-solution.png)

## 欄位名稱捨棄錯誤

**錯誤碼：**
`XTK-170036 Unable to parse expression 'i__name'`

**原因：**

失敗點可能發生在 **擴充活動**. 最常見的其中一項會顯示於下方。

![欄位名稱捨棄錯誤](/help/_assets/kt-13256/field-name-dropped-error.png)

當您手動編輯活動中的運算式名稱時，就會發生這種情況。 此影像顯示運算式修改自 `name `至 `i__name`.

**解決方案：**

您可以透過三種方式解決此錯誤：

1. 將名稱變回原先出現的運算式。

2. 如果您想使用新名稱，請變更 **擴充活動**.

3. 如果您不記得已變更的內容，最好是重新建立活動。

## 暫存資料表捨棄錯誤 

**錯誤碼：**
`XTK-170024 The temporary schema "temp:deliveryEmail1" is not defined in the current context.`

**原因：**
這是涉及擴充或其他活動的複雜工作流程中的常見錯誤。 這可能表示在對工作流程進行多項變更期間，部分活動工作流程未正確儲存。

![暫存資料表捨棄錯誤 ](/help/_assets/kt-13256/temp-table-dropped-error.png)

**解決方案：**
此錯誤發生的方式有很多種，因此沒有簡單的修正方法。 如果是簡單的工作流程，則最好重新設定活動。 在複雜的工作流程中，最好將工作流程活動複製到新工作流程，然後儲存並重新執行。
