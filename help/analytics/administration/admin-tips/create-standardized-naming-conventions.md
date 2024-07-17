---
title: 建立標準化的命名慣例
description: 標準化的命名慣例適用於變數名稱本身（在AA管理員UI中啟用時）以及傳遞到維度的值。
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
source-git-commit: c568ed0a06551d910b6f533698ec47c15adecf6c
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 建立標準化的命名慣例

**主題：**&#x200B;標準化的命名慣例適用於變數名稱本身(在[!DNL Adobe Analytics] (AA)管理員UI中啟用時)以及傳遞到維度的值。 (也就是頁面名稱會以「頁面名稱(v1)」作為變數名稱，而傳入的頁面名稱值應該是統一的且遵循特定的結構/階層，例如「sitename|homepage」或「sitename|search|searchresults」)。

**理由：**&#x200B;命名慣例是保持一切專案統一，並讓使用者容易瞭解介面的好方法。 如果您從一開始就建立慣例並在平台和程式碼中強制執行，會比較容易規模化。

**做法：**&#x200B;介面和標籤檔案應同時符合「名稱」和「說明」 — 這讓您的使用者不必提取Excel檔案，並能在介面中直接理解您的資料。 此外也建議所有內容採用小寫，以維持一致性。

最好在整個平台上保持頁面名稱一致（或應用程式的熒幕名稱）。 例如，您可以將&quot;`property:section:sub section:sub sub section:unique page name`&quot;設定為變數/維度。 如果以上這些都是資料層中的單獨欄位，您甚至可以直接在JS檔案/Launch中建置頁面名稱。 將所有這些元素都設定在其本身的維度中，可協助您更輕鬆地劃分網站/應用程式的特定屬性或區域，以及更能瞭解流量和流程。

任何可讓使用者更容易找到並瞭解資料的內容（包括一些簡單的命名慣例）都會增加[!DNL Adobe Analytics]的使用量，並為企業提供更好的深入分析。

## 作者

本文的共同作者為：

![Christel指南](assets/Christel-Headshot-150.png)

NortonLifeLock的數位[!DNL Analytics]平台管理員Christel Guidon
[!DNL Adobe Analytics]冠軍

![Rachel Fenwick](assets/Rachel-Fenwick-150.png)

[!DNL Adobe]資深顧問Rachel Fenwick
