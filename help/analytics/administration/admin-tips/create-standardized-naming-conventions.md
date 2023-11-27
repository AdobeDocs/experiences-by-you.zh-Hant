---
title: 建立標準化的命名慣例
description: 標準化的命名慣例適用於變數名稱本身 (在 AA 管理員 UI 中啟用時) 以及傳遞到維度的值。
solution: Analytics
feature-set: Analytics
feature: Implementation Basics
topic: Administration
role: Admin
level: Beginner
doc-type: article
thumbnail: 10531.jpg
kt: 10531
exl-id: 79cec21e-2b52-4e7b-88ad-db137a8cef4e
source-git-commit: 058d26bd99ab060df3633fb32f1232f534881ca4
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 80%

---

# 建立標準化的命名慣例

**內容：** 標準化的命名慣例適用於變數名稱本身，但需在中啟用 [!DNL Adobe Analytics] (AA)管理員UI和傳遞到維度的值。 (也就是頁面名稱會以「頁面名稱 (v1)」作為變數名稱，而傳入的頁面名稱值應該是統一的且遵循特定的結構/階層，例如「sitename|homepage」或「sitename|search|searchresults」)。

**理由：**&#x200B;命名慣例是保持一切項目統一，並讓使用者容易了解介面的好方法。 如果您從一開始就建立慣例並在平台和程式碼中強制執行，會比較容易規模化。

**做法：**&#x200B;介面和標記文件應同時符合「名稱」和「說明」- 這讓您的使用者無須提取 Excel 文件，並能在介面中直接理解您的資料。 此外也建議所有內容採用小寫，以維持一致性。

最好在整個平台上保持頁面名稱一致 (或應用程式的螢幕名稱)。 例如，您可以將「property:section:sub section:sub sub section:unique page name」設定為變數/維度。 如果以上這些都是資料層中的單獨欄位，您甚至可以直接在 JS 檔案/Launch 中建置頁面名稱。 將所有這些元素都設定在其本身的維度中，可協助您更輕鬆地劃分網站/應用程式的特定屬性或區域，以及更加了解流量。

任何可讓使用者更容易找到並瞭解資料的內容（包括像命名慣例這樣簡單的內容）都會增加的使用量， [!DNL Adobe Analytics] 並為企業提供更佳的見解。

## 作者

本文的共同作者為：

![Christel Guidon](assets/Christel-Headshot-150.png)

Christel Guidon，數位 [!DNL Analytics] NortonLifeLock的平台管理員
[!DNL Adobe Analytics] 冠軍

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

 資深顧問 Rachel Fenwick[!DNL Adobe]
