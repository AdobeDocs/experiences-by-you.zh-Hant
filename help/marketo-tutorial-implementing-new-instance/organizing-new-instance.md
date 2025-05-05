---
title: 組織新執行個體並建立命名慣例
description: 瞭解如何在您的Marketo Engage執行個體中設定良好的組織，好讓組織內的未來行銷人員輕鬆地瀏覽計畫、修改資產和提取報告。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03T00:00:00Z
jira: KT-14813
thumbnail: KT-14813.jpeg
exl-id: 19b3de9e-53f3-4308-b46e-7b8f756c30a0
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 2%

---

# 組織新執行個體並建立命名慣例

作為實作新Marketo Engage例項的管理員，您為未來組織內的行銷人員可輕鬆導覽該例項奠定了基礎。 熟悉樹狀資料夾結構和命名慣例可讓您的執行個體保持整潔並設定為長期成功。 本教學課程包含Adobe與Marketo Engage達人(2019-2020) Natalie Kremer建議的範例，可協助您[一致地組織資料夾並命名資產](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"}。

## 為何需要建構資料夾並套用命名慣例？

在執行個體中保持井然有序，可讓您和您的同事輕鬆追蹤行銷活動、方案和資產，並報告方案績效。 若要組織執行個體中的導覽樹狀結構並大規模建置，建議使用[資料夾](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}、[標準命名慣例](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"}以及[複製](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"}等功能。

## 如何組織Marketo Engage例項

>[!VIDEO](https://video.tv.adobe.com/v/3428941/?quality=12&learn=on&captions=chi_hant)

### 步驟1 — 設定檔案夾結構以整理您的程式

組織執行個體的第一個步驟是[設定資料夾結構](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html?lang=zh-Hant)以易於找到且有序的方式存放您的程式和資產。

在樹狀結構中建構資料夾時，以下是一些快速秘訣：

* 維持可發現性的平面資料夾結構。
* 建構您的資料夾以反映組織的團隊結構（例如地區或團隊）或方案（例如電子報）。
* 包含以時間為基礎的標籤，以啟用可搜尋性，並代表封存的適當時間（例如2024）。
   * 建議管理員每年至少封存資料夾一次。 使用年度資料夾名稱，您可以輕鬆停用即時Smart Campaigns，並在年底封存整個資料夾。

以下是將這些秘訣付諸實踐的檔案夾範例。

樹狀結構中的&#x200B;**資料夾名稱**

>[!BEGINTABS]

>[!TAB 行銷活動]

![資料夾行銷活動](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB 設計工作室]

![資料夾設計工作室](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB 資料庫]

![資料夾資料庫](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### 步驟2 — 在程式中建置資料夾

現在，讓我們在方案層級套用資料夾結構。 將本機資產放在子資料夾中，會是最理想的作法，可協助您保持程式整齊，並允許內部使用者有效率地修改或報告程式。 常見的子資料夾包括電子郵件、登陸頁面、智慧行銷活動、清單、報告等。

**程式內的資料夾名稱**
* 行銷活動 — *所有管理互動和狀態追蹤之行銷活動的資料夾。*
* 本機Assets - *此程式專屬之所有資產的資料夾。*
   * 電子郵件
   * 登陸頁面
   * Smart Campaign
   * 清單 — *只有存在程式特定清單時才需要。*
   * Forms - *只有在有特定於計畫的Forms時才需要；大多數Forms都是全域Assets。*
   * 報告 — *只有存在程式特定報告時才需要。*

### 步驟3 — 建立程式和資產的命名慣例

在樹狀結構中建立資料夾結構後，您會想要以一致的方式為程式和資產命名。 這是標準化命名慣例有助於在內部擴大命名流程的時間。 以下是可用來建立命名慣例以確保可搜尋性的幾個元件：

* 計畫型別縮寫 — 電子郵件、內容、Nurture、網路研討會等。
* 類別 — 方案型別 — 獨立電子郵件、電子報等。
* 日期 — 方案啟動日期
* 簡短說明 — 方案的簡短說明

現在，讓我們將值放入公式中，並產生各種程式型別的程式名稱。

#### 程式命名公式

| **程式型別**&#x200B;的縮寫 | **YYYY** | **\-** | **毫米** | **\-** | **DD（選擇性）** | **類別** | **\-** | **程式的簡短描述** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| EM — 電子郵件傳送（電子郵件程式） | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| NL — 電子報 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| ENG — 參與計畫 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| WBN — 網路研討會 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| IW — 互動式網路研討會 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| TS — 商展 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| LE — 現場活動（路演） | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| UG — 使用者群組 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| WC — 網站內容 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| CS — 內容整合 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| LI — 清單匯入 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| OA — 線上Advertising | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |
| PPC — 每次點按付費 | YYYY | \- | 公厘 | \- | DD （可選） | 類別 | \- | 計畫的簡短描述 |

| **範例** |
| --- |
| ES 2023-10閘道內容 — XYX白皮書 |
| WC-2023-10 — 每月網路研討會 — ABC個案研究 |

#### 資產命名公式

向下移至命名資產的一個層級，最好不要重複程式名稱，並使用簡短和通用識別碼以利日後的複製使用。 以下提供一些快速秘訣，請您牢記在心：

* 根據資產在方案程式中的順序對其進行編號。
* 使用「 — 」（連字型大小）來區隔命名元件，而非「。」（點）或「\_」（底線）。
   * 為什麼？ Marketo Engage使用點將「方案名稱」與「促銷活動名稱」隔開。 使用「\_」會在資產超連結時防止您看到它。
* 在資產名稱中使用標準首字母縮寫來縮短參照，同時仍可輕鬆辨識。

有鑑於此，我們會將這些秘訣套用至下列資產，並建立公式以產生名稱：

##### 根據計畫程式中的順序命名資產

| **程式處理序中的順序** | **\-** | **說明** |
| --- | --- | --- |
| 01 | \- | 說明 |
| 02 | \- | 說明 |
| 03 | \- | 說明 |

| **範例：智慧清單** |
| --- |
| 01 — 傳送電子郵件 |
| 02 — 已開啟 |
| 已點按03 |
| 04位填寫的表單 |
| 05受影響（計畫成功） |
| 06 — 已取消訂閱 |

##### 使用資產型別的縮寫來命名資產

| **資產型別**&#x200B;的縮寫 | **資產型別** | **\-** | **目標**&#x200B;的說明 |
| --- | --- | --- | --- |
| LP — 登陸頁面 | LP | \- | 目標的說明 |
| 電子郵件 — 電子郵件（傳出） | EMAIL | \- | 目標的說明 |
| 警報 — 電子郵件警報 | 警報 | \- | 目標的說明 |
| WF — 網路表單 | WF | \- | 目標的說明 |
| EXCL — 排除清單 | 不包括 | \- | 目標的說明 |
| SLST — 智慧清單 | SLST | \- | 目標的說明 |
| LST — 靜態清單 | 清單 | \- | 目標的說明 |

| **範例** |
| --- |
| LP註冊 |
| LP-ThankYou |
| 電子郵件 — 傳出 |
| 電子郵件 — 電子報 |
| 電子郵件邀請 |
| 電子郵件提醒 |
| EXCL競爭者 |

##### 使用資產型別的縮寫來命名可下載的檔案(.pdf)

| **資產型別** | **內容描述** | **\-** | **資產型別**&#x200B;的縮寫 | **.** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP — 白皮書 | 內容說明 | \- | WP | 。 | pdf |
| CS — 個案研究 | 內容說明 | \- | CS | 。 | pdf |
| DS — 資料表 | 內容說明 | \- | DS | 。 | pdf |

| **範例：可下載的PDF檔案** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>在上述範例中為檔案命名時，請勿使用空格並避免使用底線「\_」

## 接下來呢？

* 下載工作表：[Marketo Engage組織和命名慣例](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"}以支援建立資料夾結構和命名慣例。
* 決定標準命名慣例中的必要元件後，請考慮將公式建置到Google工作表或Microsoft Excel中。 若日後使用，只需在試算表中輸入您的值，即可產生您的程式名稱。
* 一旦您調整好整體檔案夾結構，您就可以根據最常見的使用案例和團隊最常收到的請求，來思考您需要的範本。 然後開始建立您的第一個方案範本。 請閱讀以開始使用[Adobe Marketo Engage方案範本](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}。

### 作者

{{natalie-kremer}}

{{amy-chiu}}
