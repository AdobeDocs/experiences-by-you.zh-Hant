---
title: 從Google [!DNL Analytics]轉換成 [!DNL Adobe Analytics] 的全方位指南
description: 瞭解同等功能的位置，以及從Google [!DNL Analytics] 轉換到 [!DNL Adobe Analytics]時如何有效使用該功能
solution: Analytics
feature: Third-party Integration
role: User
level: Beginner
kt: 9830
thumbnail: 34749.jpg
exl-id: 646bdc8f-c95e-40be-b2f7-8e4ba5653d91
source-git-commit: 02e3a6dfa59df45113242bd8e874e18e9e1efd58
workflow-type: tm+mt
source-wordcount: '3323'
ht-degree: 0%

---

# 從Google [!DNL Analytics]轉換成[!DNL Adobe Analytics]的全方位指南{#comprehensive-guide-for-transitioning-to-adobe-analytics}

## 1.簡介

在任何工具之間轉換的最大挑戰之一，就是瞭解應在何處找到同等功能，並瞭解如何有效率地使用它。 此討論內容是幫助使用者更輕鬆地轉換到[!DNL Adobe Analytics]的大型指南的一部分(可以是新的使用者，也可以是來自Google [!DNL Analytics]的使用者)。 提供與GA的深入比較（這是大多數使用者最有可能熟悉的比較工具），以協助使用者將現有知識與新工具集建立關聯。 若沒有替代做法，這有助於您開始使用並減少您在此期間可能會遇到的挫敗感。

我們應該快速比較一下術語：

| **說明** | **[!DNL Adobe Analytics]** | **Google[!DNL Analytics]** |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------------|
| 代表某個頁面（或應用程式上的某個畫面）已被檢視的事件量度 | 頁面檢視 | Pageview |
| 代表您的網站或應用程式上發生在相同時間範圍內的一組互動的量度 | 造訪 | Session |
| 定義已識別之裝置的量度（根據多個條件，包括Cookie和其他行為模式以拼接使用者資訊） | 不重複訪客 | 使用者 |

## 2.介面

當人員比較[!DNL Adobe Analytics]和Google [!DNL Analytics]時，他們的註解是[!DNL Adobe]的介面剛開始會令人生畏。 這是真的，但信不信由您，這也是一種優點，而不是弱點。 [!DNL Adobe]為您的資料視覺化提供各式各樣的工具和靈活性，讓您有更多自由建立所需的資料。

讓我們從檢視「網站內」報告開始。

### 2.1.網站內報告

#### 2.1.1.首頁畫面

[!DNL Adobe Analytics]和Google [!DNL Analytics]都有提供方式讓您自訂使用者登入時最先看到的檢視畫面。

##### 2.1.1.1. Workspace /自訂首頁畫面([!DNL Adobe Analytics])

[!DNL Adobe Analytics]不會擅自為所有登入的使用者預先建立報表以供他們檢視。 預設首頁會帶領使用者前往Workspace登陸畫面，該畫面會向每位使用者顯示他們所建立或是他人與其共用的所有工作區報表。 此外，每個使用者也能選擇將任何報表設定為首頁。

![workspace-create-project](assets/ga-to-aa_1.png)

本指南的稍後章節會提供有關工作區的更多詳細資訊。 請參閱第2.1.2.1小節

>[!TIP]
>
>為貴組織建立/共用一些標準報表，好讓他們有一個起點可檢視資訊，而不必立即著手建立自己的報表。



##### 2.1.1.2.首頁畫面深入分析(Google [!DNL Analytics])

* Google [!DNL Analytics]首頁畫面已為您預先建立一些視覺效果。 其中涵蓋：
* 過去七天的使用者、工作階段、跳出率和工作階段持續時間
* 依據一天當中的時間列出過去30天的使用者
* 目前的使用者以及最活躍的頁面
* 過去七天的流量管道、Source/Medium和轉介
* 依國家列出過去七天的工作階段
* 過去七天的熱門頁面
* 過去30天的活躍使用者趨勢
* 及更多內容

GA4使用者有更多選項，可自訂首頁畫面並將自己的報表新增到該畫面。

![google-analytics-interfaces](assets/ga-to-aa_2.png)

這可能是您對[!DNL Adobe Analytics]最懷念的一件事。 沒有為您預先建置的首頁畫面。 不過，您可以輕鬆設定自訂Workspace，從上述清單中複製您需要的內容，並將其設定為您的登陸畫面。 稍後會提供更多相關內容(或請參閱第2.1.2.1小節[!DNL Adobe] Workspace)。

#### 2.1.2.網站內Report Builder

除了分析工具提供的簡單報表之外，每個工具也提供更強大的工具，讓您可用來建置自己的自訂報表。

##### 2.1.2.1。[!DNL Adobe Analytics] Workspace

這是[!DNL Adobe Analytics]的動力來源，自從它在2017年推出以來，就成為了[!DNL Analytics]分析的首選之地，也是「報表」區段即將成為明日黃花的主要原因。

此工具讓您在建立報表時幾乎擁有完整的自由度。

報表可以分成多個面板，而這些面板可包含任意數量的視覺效果。 面板可以設定為常用資訊，例如日期範圍和常用區段篩選器。

面板及其中的視覺效果都可以調整大小並四處拖曳，以並排或棧疊方式顯示專案。 因此，如果您想要並排比較兩套不同的資料，可以建立以50/50方式在中間拆分的面板，並排顯示兩個網站以方便比較。

有許多視覺效果可供使用者使用：

* 自由表格
* 同類群組表格
* 流失
* 流程
* 圖表
   * 區域圖（棧疊和非棧疊）
   * 折線圖
   * 散佈圖
   * 橫條圖（棧疊和非棧疊）
   * 專案符號
   * 環狀
   * 長條圖
   * 水準橫條圖（棧疊和非棧疊）
* 地圖
* 摘要區塊
   * 摘要變更
   * 摘要文字
   * 文字（可輸入額外資訊以提供內容的任意文字欄位）
* 文氏圖表

每個面板和視覺效果都可以加上標題並套用說明，以提供上下文幫助使用者瞭解所顯示的資訊。
在[!DNL Adobe]中，區段（基本上是資料的篩選器）可回溯套用，而且這些區段可以拉取至自由表格中的欄，以便並排比較資料。 例如，如果使用者想要比較其網站上兩個不同類別的流量，他們可以為「類別A」建立一個區段，並為「類別B」建立另一個區段。

![analytics-page-views-report](assets/ga-to-aa_3.png)

自由表格可讓您視需要建立多個欄和分段，以便依您想要的方式將資料視覺化。

如果您不想要依日期檢視劃分，只需將另一個維度或區段拖放到那裡，以不同的方式檢視資料。 例如，為「裝置型別」使用區段，然後為您的行動/平板電腦使用者依作業系統新增劃分：

![analytics-compare-page-views-report](assets/ga-to-aa_4.png)

Workspace可讓您自由發揮創意，不限於「標準」劃分。 您可以建立所需的視覺效果，以深入探究您需要進行的比較。

>[!TIP]
>
>不用害怕實驗和探索。 有許多方式可跳出框架思考。 此外，可驗證您建置的內容是否說明了您的想法。 經驗很有幫助！

您可以建立僅存在於報表中的動態計算量度或區段，以防止溢位您的區段和計算存放庫。 這可讓您建立特定報告所需的重點專案，而不會將您的組織與其他內容中無法使用的東西混淆。

本討論內容只是為了介紹這個工具，還有其他完整的指南可協助您開始使用。 檢閱這些指南後，您將製作以下綜合報表：

![workspace-dashboard](assets/ga-to-aa_5.png)

工作區不會自動儲存，所以進行一次性的臨時報告會比較容易，這樣就不會塞滿報表存放庫。

工作區有另一個強大的功能，就是能夠以下拉清單的形式將互動式修飾詞套用到您的報表。 這些下拉式清單並不適用於匯出的CSV或報表的PDF檔案。 不過，在即時報表中，上述功能可讓您更新面板中的所有視覺效果，以在不同條件下顯示相同報表。 您可以使用多個下拉式清單，而且只要選項不互斥，選取的專案就會棧疊起來，能以簡潔的方式呈現資訊。

>[!IMPORTANT]
>
>若要進一步瞭解如何使用下拉式清單和自由格式劃分，請參閱<https://experienceleaguecommunities.adobe.com/t5/adobe-analytics-discussions/the-power-of-dropdown-filters-and-dimension-breakdowns-in-adobe/td-p/434680>

##### 2.1.2.2. Google [!DNL Analytics]：儀表板、自訂報表和已儲存報表

Google有一些工具可以在介面中建立報表，但還是要遵循報表區段的相同顯示方式和限制。

現在，對於精通Google [!DNL Analytics]的人來說，當您讀到這段文字時，您可能會說：「等等，Google Data Studio呢？它不是相當於[!DNL Adobe]的Workspace的更好嗎？」 是的，但技術上來說，Data Studio不是[!DNL Analytics]工具的一部分，而且可連線到不同的資料來源。 此工具稍後將在「擴充的報表存取」一節中介紹，尤其是第2.2.3節。

Google儀表板和自訂報表可讓您將多個視覺效果一起提取到一個報表中，但不同於Workspace，您仍然受限於簡單的關聯性以及可將哪些資料放入哪些欄。

在自訂報表中，最大的挑戰之一是當您建立篩選器時，篩選器會套用至報表的所有索引標籤。 無法在同一份報表中比較兩個不同的篩選器。

如果是表面的比較，就行得通。 這些全都類似於[!DNL Adobe]舊式儀表板、自訂報表和書籤。 提供基本工具是為了支援您在報表套裝中的需求。

#### 2.1.3.報表

Google和[!DNL Adobe]都有一些可導覽的報表，這些報表是根據維度的隨建表格及基本時間軸圖表。

##### 2.1.3.1. [!DNL Adobe Analytics]報告

[!DNL Adobe Analytics]也有「報表」區段，儘管這正被逐步淘汰，取而代之的是Analysis Workspace。 事實上，由於Workspace是更強大的工具，因此已宣佈終止使用該介面。 這些表格中的大多數都可以更輕鬆地建置和修改。 [!DNL Adobe]的區段劃分更為細分，這可能令人生畏：

![analytics-site-metrics](assets/ga-to-aa_6.png)

上述的大多數內容都可透過工作區存取，我會簡短概述這些區段以及它們與Google [!DNL Analytics]的關係，並強調在此依然相關的報告。

網站量度是您期望的，這涵蓋標準量度（頁面檢視、不重複訪客、造訪以及您已設定的自訂事件）。 這類似於行為報表GA，但也包含一些您在「對象」中可以找到的量度（因為[!DNL Adobe]不會分割量度型別）。

在這裡，您可以找到「機器人」報表。 您的所有標準報表都會排除來自機器人的流量，不過，有兩個報表可讓您深入瞭解正在發生的事情以及哪些機器人正在瀏覽您的網站。 如果您設定自訂機器人規則來排除經常造訪您網站的已知垃圾訊息機器人，這會特別有用。 您可以獲得這些機器人正在做什麼的洞察資訊，但又不會讓這些流量在您的主要報表中泛濫。 目前無法透過Workspace取得機器人報表（但即將推出的新報表功能也可讓使用者在該處取得此資訊）。

網站內容是一組[!DNL Adobe]標準維度：頁面名稱、網站區段、階層、伺服器等。 所有這些維度都可以在Workspace中使用。

「行動」是一組行動裝置特有的資料，包括裝置、裝置型別等。 這些功能在Workspace中提供。

Workspace中不提供路徑。 Workspace有一個流量圖，您可以在其中檢視單一頁面/值的輸入和輸出流程。 相反地，路徑則可讓您檢視網站中最常用的路徑。 依預設，「頁面」是為您設定的第一個路徑報表。 不過，您可以為自訂Prop （例如「頁面型別」值）開啟此功能。 您可以檢視頁面型別中的路徑分析。 我個人喜歡「路徑」的另一個原因是因為這是簡單的資訊呈現方式……工作區中的流程圖表（取決於您要檢視多少內容）可能會讓人吃不消。 我建議您兩者都試試……視您嘗試達成的目標而定，它們都有用途和價值。 請注意，任何維度都可以在「流程」中使用，但「路徑分析」則必須在管理員面板中的Prop上設定。

流量來源、[!DNL Campaign]和行銷管道報表都類似於Google產品的贏取報表。 流量來源聚焦於實際反向連結、[!DNL Campaign]聚焦於您的[!DNL Campaign]程式碼，而行銷管道也聚焦於的[!DNL Campaign]程式碼，但也會套用您決定的有關資訊處理方式的額外邏輯。 [!DNL Adobe]在如何設定規則方面提供了更多自由。 相反地，Google則為您完成許多工作，這是思維的轉變。 依預設，Google對[!DNL Campaign]程式碼的歸因為六個月。 [!DNL Adobe]的歸因預設為一週。 您可以在管理員設定中加以變更，但在Workspace中，您實際上可以在任何維度之上套用自訂歸因，為您提供更大的「即時」靈活性。

「訪客保留率」和「訪客資料」報表類似於Google [!DNL Analytics]中的「對象」報表。 「訪客保留率」比較關注回訪頻率，而「訪客資料」則比較關注使用者的地理位置和技術。

自訂轉換和自訂流量報表都是自訂維度報表。 轉換則是eVar。 您可以設定該值的自訂到期時間，例如點選、造訪、月份、年份等。 除非被覆寫，否則在設定的時間段內，這個值將持續為使用者保留。 流量變數屬於prop。 您也可以為「路徑報表」設定這些變數，或將其設定為清單專案，這將根據您選擇的分隔符號拆分多個值。

「媒體」適用於您設定了特殊媒體追蹤的視訊或音訊等檔案。

「自訂報表」是使用者可以在其中自訂欄和劃分的區段，他們已在報表介面中建立這些欄和劃分，並將其儲存為自訂報表。 不過，如上面所述，由於Workspace允許更強大的劃分和關聯，因此任何自訂作業都應該在那裡進行。 在Workspace出現之前，這是一個很好的解決方案。

「書籤」區段類似於「自訂報表」，可以在報表介面中為常用的報表新增書籤，以便可以更輕鬆地找到它們。

「儀表板」是舊版產品，可讓使用者將資料的小報告一起合併到一個視覺效果中。 不過，Workspace中的功能（第2.1.2.1小節）使用起來要容易得多，它只會當作存取點存在，讓人存取在此功能被淘汰之前應該重建的舊式報表。

目標可讓人們在特定時間範圍內根據目標建立報告。 團隊監控行銷活動，以檢視他們是否有望達到流量目標。

這裡的所有報表都允許多個量度欄和維度劃分。 不過，視覺效果的簡單性以及哪些元素可以建立關聯的一些背後邏輯有時可能會讓人感到挫折。

##### 2.1.3.2. Google [!DNL Analytics]報表

Google [!DNL Analytics]將這些報表拆分成以下區段：即時、目標對象、攬客、行為和對話（在GA3中），並拆分成生命週期（包含子區段：攬客、參與度、營利、回訪率）和使用者（包含子區段：人口統計和技術）。

![google-analytics-interface-compare](assets/ga-to-aa_7.png)

您可以對這些視覺效果進行一些細微調整、新增次要維度劃分、變更視覺效果、建立資料篩選器等。 您可以將自訂內容儲存為「已儲存的報表」。

這些可讓您輕鬆快速地深入分析資料。 不過，您無法將「使用者」之類的資料與相同表格中頁面的頁面檢視進行比較，也無法新增一個以上的額外維度來檢視其他資料。

這些對於快速分析資料很有用，但如果您真的需要深入挖掘，則會受到限制。

### 2.2.擴充的報表存取

除了「網站內報告」以外，大多數的工具也提供擴充功能，好讓您可以在工具外面進行分析，並打造一些更客製化的東西。

#### 2.2.1. [!DNL Adobe Analytics]Report Builder(Microsoft® Excel副檔名)

Workspace是一個絕佳的工具，但有時您需要將資料放入自訂試算表中，這樣您就可以將多個資料來源拼接在一起。 這就是Report Builder發揮作用的地方。

Report Builder是Microsoft® Excel的外掛程式，可讓您建立與[!DNL Adobe Analytics]資料的連線，以提取您可以在Excel中操作的表格資料。 通常為了有效率地使用它，您會將資料提取到某些原始資料索引標籤中，然後使用Excel儲存格參照將這些索引標籤中的資料提取到單一整合式報表中，接著建立圖表和視覺效果。

>[!NOTE]
>
>Report Builder具有特殊許可權，需要為您的使用者套用這些許可權才能存取此外掛程式。 應將此許可權授予已瞭解如何正確使用此工具的使用者。

#### 2.2.2. [!DNL Adobe Analytics] API連線

如果您需要[!DNL Adobe Analytics]資料由Excel以外的其他程式所消化，而且您想要處理的資料包含機器人規則排除專案，請使用[!DNL Adobe]的API直接提取資料。 然後，使用指令碼處理資料或將其新增到資料庫以供其他系統使用。

請注意，API還是會套用提取請求中指定的劃分和區段來提取關聯資料。

[!DNL Adobe]的Workspace （第2.1.2.1小節）會使用此API來建立報表，而且如果您在Workspace中啟用偵錯模式，它會向您顯示使用的確切API呼叫。 這是建置API呼叫的快速方法。 透過使用Workspace建置及驗證您要提取的資料，您接著可使用這些API呼叫將資料取出以供您自行處理。


#### 2.2.3. Google [!DNL Analytics] Data Studio

如果您一路閱讀下來，就會知道我在上面提過Data Studio的作用等同於[!DNL Adobe]的Workspace。 Data Studio可讓您提取Google [!DNL Analytics]資料，但也可提取其他來源的資料。 如果您想要將分析資料與其他收集的資料合併，這是不錯的做法。 但是，若使用Google [!DNL Analytics]，則會出現相同型別的視覺效果限制。 列和欄的形成方式仍然受限。

這仍然是一個強大的工具，我不會勸阻人們以任何方式使用它。 我個人的經驗是，我發現僵化的行為相當有限。


#### 2.2.4. Google試算表擴充功能

針對我自己的用途，當我需要以擴充方式從Google [!DNL Analytics]提取資料時，我個人選擇的工具是Google試算表擴充功能。 即使我需要和我的GA表格建立多個連線，我可以從原始資料中參照儲存格並建置我需要的報表。 接著，我使用Google試算表的繪圖功能將其視覺化。


## 3.原始資料匯出

當您真正需要原始資料時，[!DNL Adobe]和Google都有提供以這種方式提取資訊的功能。

### 3.1. [!DNL Adobe]資料摘要

在第2.2.2小節中，我提到[!DNL Adobe Analytics] API會從「處理的資料」中提取。 原始資料摘要會提取已在管理面板中設定的「處理規則」所處理的資料，但此原始資料會包含其他任何地方都已排除的所有資料。

這表示您的所有機器人擴充功能、內部IP篩選的資料以及其他已排除資料都會納入原始資料摘要中。 有旗標可識別這些資料，因此如果您建立Data Lake，工程團隊可建立邏輯以相應地處理這些資料。

您可以自訂原始資料摘要，以傳送所有資料欄，或是在您需要更聚焦的摘要時僅傳送特定欄。

摘要可以直接傳送給FTP、SFTP或S3。


### 3.2. Google Big Query

遺憾的是，我還沒有用過這個Google工具。 理論上，它應該類似於[!DNL Adobe]的資料摘要，可讓您的工程團隊存取您Google [!DNL Analytics]帳戶的原始資料。

不過，與其提供完整的原始資料傾印，它可讓工程師透過SQL查詢存取資料，以提取目標原始資料或所有原始資料欄。

## 4.結論

像任何系統一樣，需要練習才能熟悉該工具。 希望本指南可協助您開始使用，或提供提示以改進您對[!DNL Adobe Analytics]的使用。

不過我要強調，我建議在您的實作策略中同時使用[!DNL Adobe Analytics]和Google [!DNL Analytics] (即使Google [!DNL Analytics]僅為免費版本)。 這可讓您擁有備份系統，以確保您擁有資料，因為沒有任何系統是萬無一失的。

除了本指南以外，還有許多資源可幫助您改善策略：

* [[!DNL Adobe] Experience League](https://experienceleague.adobe.com/zh-hant#home) — 包含教學課程、影片、檔案和社群論壇
* [[!DNL Adobe] 使用者群組](https://analytics-augs.adobe.com/) — 這是社群開展活動的中樞，可幫助使用者互相交流並改善其實作。
* [[!DNL Adobe Analytics] 使用者群組YouTube頻道](https://www.youtube.com/channel/UCQOHnCs7KZgsuFHVzwboQuA) — 無法加入[!DNL Adobe Analytics]使用者群組工作階段？ 重新觀看先前全球使用者群組時段內容，瞭解更多關於您的同業如何使用該工具。
* [Measure ChatSlack頻道](https://www.measure.chat/) — 與全球[!DNL Adobe Analytics]位使用者交流，並分享業界學習經驗、向同業請教，並加入衡量主要利益群組。
* 及更多內容！

## 作者

本檔案的作者為：

![Jennifer Dungan](assets/Jennifer_Dungan_Headshot150.png)

Jennifer Dungan，最佳化經理[!DNL Analytics] at Torstar

[!DNL Adobe Analytics]冠軍
