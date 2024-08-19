---
title: 使用Dynamic Chat設計全通路對話式行銷
description: 透過Adobe Marketo Engage中的原生對話式參與管道Adobe Dynamic Chat，快速開始設計對話式行銷。 本教學課程提供實作使用案例的可操作方法，例如銷售會議預訂、網站內容參與和活動/網路研討會促銷活動。
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-23T00:00:00Z
jira: KT-14814
exl-id: 160dfb25-9f54-4dce-a08a-4a8d3c4c5368
source-git-commit: 1205848b1985a99b91f9d4d25e1a79f0df379589
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# 使用Dynamic Chat設計全通路對話式行銷

行銷人員您的網站對於創造銷售機會、提高轉換率並加快銷售週期至關重要。 透過即時接觸網站上的訪客，讓您的銷售團隊更有效率地符合買家的資格。 Adobe Dynamic Chat是Adobe Marketo Engage訂閱內的原生聊天頻道，可讓您自動進行交談，以擴充Marketo Engage的功能。

本教學課程概述思維和主要使用案例，由Cornerstone OnDemand行銷營運經理Sara Barriuso在「向同行學習」期間分享。 她說明她的組織如何使用Dynamic Chat來充份發揮Marketo Engage的功能。

## 將對話式參與整合至您的需求產生策略

訪客瀏覽您的網站是有原因的。 他們可能會尋找您產品或服務的內容，或尋找聯絡資訊以便與您的銷售代表交談。 他們也可能是在尋找其他產品資訊的客戶。 如果網站訪客準備好與您的銷售團隊交談，聊天功能可讓他們自助服務並取得資格。

當Sara Barriuso實作Dynamic Chat時，她被其與Marketo Engage的緊密整合以及啟動Marketo Engage程式的[預先建置的活動觸發器](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target="_blank"}所吸引，反之亦然。 她針對三個受眾區隔制定了對話式參與策略：

1. 未知的潛在客戶：主動提供示範呼叫，以產生新的潛在客戶。
2. 已知銷售機會/客戶：延長訪客瀏覽內容所花的時間，並提供示範電話來產生向上銷售和交叉銷售機會。
3. 潛在客戶/客戶：透過擴展行銷活動的力度，提供個人化體驗。


## 開始建立對話方塊的主要使用案例

為了實作這些策略，Sara圍繞以下使用案例建立了她的Dynamic Chat對話方塊：

1. 預設全域對話方塊：為所有訪客提供初始選項，引導他們更有效地完成任務。

2. 推廣活動和網路研討會報名：推動網站訪客報名參加活動和網路研討會，讓他們更快進入購買階段。

3. 擴大促銷活動內容參與度：提供額外內容，或解決訪客瀏覽網站內容時的潛在問題。

讓我們在Sara展示其流程時，看看這些使用案例的實際運作情形。從對應對話流程，到設定對話方塊，以及在Dynamic Chat和Marketo Engage中進行目標定位。

### 使用案例1：所有網站訪客的預設全面對話方塊

此對話方塊提供五個初始選項供網站訪客選擇，建立自助式體驗，協助他們根據角色尋找所需的資訊。 若要開始，您可能會想要探索「聯絡我們」電子郵件收件匣，以識別常見的主題並將其分類為適用於網站訪客的對話方塊選項。 觀看示範，然後依照下列步驟建立您的預設全包式對話方塊：

>[!VIDEO](https://video.tv.adobe.com/v/3429194/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### 階段1

1. 建立對話方塊並建立測試連結。
2. 新增目標以追蹤轉換（例如示範要求提交）。
3. 讓2至3名人員測試並收集意見回饋。

#### 階段2

1. 在「對象」中，於「目標」中新增網頁URL，以指出對話方塊會出現的位置。
2. 在「設定」中，新增行銷活動名稱、說明、優先順序和語言。
3. 按一下「Publish」

>[!TAB Marketo Engage]

#### 階段1

1. 建立您的追蹤Smart Campaign。
2. 在「智慧清單」中，使用「到達對話方塊目標」觸發器。 使用您使用的對話方塊中的相同目標（例如示範請求）
3. 在「流量」中，加入「變更方案狀態」步驟以追蹤轉換。
4. 來源會顯示為「dynamicChat」。 您可以建立Smart Campaign，將來源更新為您認為合理的名稱。

#### 階段2

1. 請在您的追蹤Smart Campaign上線時重新測試。

>[!ENDTABS]

#### 提升：帳戶型行銷

您可以結合產業目標式內容，進一步增強預設的全方位對話方塊，讓對話對訪客更有用。 例如，建議下載特定產業白皮書或個案研究。 觀看示範，並依照下列步驟建立帳戶型行銷的預設全包式對話方塊：

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. 原地複製「預設對話方塊」並重新命名。
2. 在「串流Designer」中，將Dialogue訊息調整至目標產業（只有一個串流+初始問題）。
3. 讓2至3個人測試對話方塊並收集意見回饋。
4. 建立測試連結並分享。
5. 在「對象」中，新增將顯示對話方塊的網頁URL，並將目標更新至您想要的產業。
6. 在「設定」中，新增行銷活動名稱、說明優先順序和語言。
7. 按一下「Publish」。

>[!TAB Marketo Engage]

1. 建立您的追蹤Smart Campaign並測試目標。
2. 發佈對話方塊後，重新測試追蹤Smart Campaign。

>[!ENDTABS]

### 使用案例2：推廣活動和網路研討會報名

活動和網路研討會是B2B企業產生需求的熱門行銷策略。 他們提供吸引人的體驗和豐富的資訊，吸引潛在客戶。 將您的網站訪客連結至即將舉辦的活動和網路研討會，讓您更快取得潛在客戶的資格。 建立此對話方塊可簡化工作且成本低，並可快速展示成功，協助您獲得行銷利害關係人的支援，以將對話式參與加入您的全通路自動化計畫。 觀看示範，並依照下列步驟建立您的活動/網路研討會促銷活動對話方塊：

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### 階段1

1. 建立「事件註冊」對話方塊的範本，以供持續性行銷活動使用。

#### 階段2

1. 複製範本。
2. 將文字複製並貼上新事件的對話方塊訊息
3. 更新事件連結中使用的UTM引數（例如utm_medium=website&amp;utm_source=adobe）。
4. 建立測試連結，按一下「Publish」，然後與請求者共用。
5. 同級檢閱並套用意見回饋。


>[!TAB Marketo Engage]

#### 階段1

1. 在網路研討會/活動方案範本中建立您的追蹤Smart Campaign並進行測試。

#### 階段2

1. 將您的行銷活動名稱新增至Marketo Engage中的追蹤Smart Campaign並進行測試。

>[!ENDTABS]


#### 等級：註冊已知人員

您可以為網站訪客註冊參加您的活動和網路研討會，無需他們填寫表單，即可為他們提供更好的體驗。 個人化的體驗可建立信任，並向訪客顯示您記得的訪客。 讓我們瞭解如何提升您的活動和網路研討會促銷對話方塊的實際運作水準。

>[!NOTE]
>請考量某些保護性國家/地區的潛在安全風險，並與您的法律團隊協商，謹慎實施此個人化。

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. 複製活動/網路研討會促銷活動對話方塊。
2. 在串流Designer中，使用者回答「是」後，新增問題卡「您先前曾與我們共用您的電子郵件地址。 您想要保留此專案以取得事件詳細資料嗎？」
3. 如果他們回答「是」 — 新增訊息卡「您將在您的電子郵件中收到一封包含活動/網路研討會詳細資訊的確認電子郵件」。
4. 如果他們回答「否」 — 新增訊息卡「請在註冊頁面上填寫表單」。
5. 建立測試連結，按一下「Publish」，然後與請求者共用。
6. 在[對象]索引標籤中，新增[電子郵件不是空的]。

>[!TAB Marketo Engage]

1. 新增此新的對話方塊至追蹤中的Smart Campaign，並加以測試Marketo Engage。

>[!ENDTABS]

### 使用案例3：擴充行銷活動內容參與度

想像一下，迷人的視窗顯示器能吸引您的眼球，並將您吸引到商店中。 如果接待人員接著協助您選取產品或回答您的問題，您可能會覺得更舒服地購物。 若要線上復寫此體驗，您可以讓Dynamic Chat對話方塊出現在行銷活動導向訪客的網頁上。 當使用者與網路內容互動時，Dynamic Chat會立即顯示相關對話、建議其他內容或解決潛在問題。 這是透過利用自動化觸發器，根據使用者在Dynamic Chat計畫中的參與來啟動Marketo Engage促銷活動來達成。 現在，讓我們來看看如何讓此使用案例更加生動。

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

延伸Campaign內容參與 — 設定：

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. 透過電子郵件和社交行銷活動的接觸點，為您的行銷活動產生新的銷售機會。 在此範例中，Talent健康指數調查託管於品牌的網站上。
2. 複製現有的對話方塊範本（例如預設的全方位對話方塊），為下列案例建立三個對話方塊，並相應地更新「對象」標籤中的「目標URL」：
   * 當網路訪客從您的行銷管道進入您的網頁時。
   * 在感謝頁面上
   * 任何在參與行銷活動（重新目標定位）後45天內回訪您網站的訪客

>[!ENDTABS]

## 接下來呢？

* 在[串流Designer](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target="_blank"}或離線流程圖中對應您的對話流程。
* 在Dynamic Chat中建立預設的涵蓋所有對話方塊。
* 在Marketo Engage中使用自動化觸發程式，在行銷活動後啟用交談。


## 作者

{{sara-barriuso}}

{{amy-chiu}}
