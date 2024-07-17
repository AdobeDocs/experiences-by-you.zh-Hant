---
title: 建立標準化的程式碼範本
description: 對於基準線實作（亦即貴公司認為所有 [!DNL Adobe Analytics] 網站必備的KPI），貴組織應儘可能採用單一實作方法。
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10532.jpg
kt: 10532
exl-id: edd3df73-6d1a-4a26-a984-810cc7dd382f
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# 建立標準化的程式碼範本

**主題：**&#x200B;若為「基準線」實作（亦即貴公司認為所有[!DNL Adobe Analytics]網站必備的KPI），貴組織應儘可能採用單一實作方法。 例如，跨網站使用相同的資料層結構，以及運用相同的標籤管理員規則/自訂程式碼來擷取內部搜尋或訪客資料資訊等專案。

**理由：**&#x200B;擁有可重複且可擴充的基準線實作，可簡化新增新元素或新網站/應用程式的工作，同時保持實作整潔且易於疑難排解。 使用統一的方法還能讓新的管理員/開發人員更容易上線並瞭解他們正在使用的內容。

**做法：**&#x200B;採用單一格式範本，在新網站或標籤增強功能上線時交給開發人員。 通常，Word檔案就很好用了，您可以在其中概述以下專案：

* 實施的變數、變數的用途以及何時設定。 例如：

| AA變數 | 說明 | 何時/何處設定 | 如何設定 |
|--- |--- |--- |--- |
| EVAR8 | 內部搜尋關鍵字 | 登陸內部搜尋結果頁面時 | 資料層 |
| event8 | 內部搜尋計數 | 登陸內部搜尋結果頁面時 | Launch規則 |

* 如何設定的詳細說明。 您可以在此處指定所需的任何資料層物件及其語法，以及任何需要設定的TMS規則和規則設定的詳細資料。
* 要確保的測試案例包含在QA中，以及您預期會在成功的測試案例中看到的所有變數。 概述當開發人員測試此增強功能時，成功的實作應包含哪些專案。

理想情況下，此檔案只需針對下一個網站進行調整，您可以更新屬性名稱、頁面命名慣例等基本知識。 無需每次都重複相同的步驟，您可以節省更多時間。

## 作者

本文的共同作者為：

![Christel指南](assets/Christel-Headshot-150.png)

NortonLifeLock的數位[!DNL Analytics]平台管理員Christel Guidon
[!DNL Adobe Analytics]冠軍

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

[!DNL Adobe]資深顧問Rachel Fenwick
