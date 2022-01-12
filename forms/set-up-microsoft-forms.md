---
title: 設定 Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: microsoft-365-education
ms.localizationpriority: high
description: 了解 Microsoft 365 系統管理員如何控制 Microsoft Forms 在其組織中的使用方式。 同時了解安全性與合規性問題的解答，例如 Microsoft Forms 的資料儲存位置。
ms.openlocfilehash: bb0e1a6ba8e2085550eb18a8bb393b34b197fe51
ms.sourcegitcommit: 80aa5565b4008855be844e8e5ab3f2779fba9a83
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/05/2022
ms.locfileid: "61723721"
---
# <a name="set-up-microsoft-forms"></a>設定 Microsoft Forms

## <a name="overview"></a>概觀

Microsoft Forms 可讓您的使用者快速且輕鬆地建立自訂測驗、問卷、問卷調查、註冊等等。 當您建立測驗或表單時，您可以邀請其他人使用任何網頁瀏覽器，甚至是行動裝置，來進行回應。 提交結果之後，您可以使用內建分析來評估回應。 表單資料，例如測驗結果，可以輕鬆地匯出至 Excel 進行其他分析或是評分。

若要深入了解，請參閱[什麼是 Microsoft Forms？](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) 或者，請參閱我們關於 Microsoft Forms 的 [Microsoft 365 部落格文章](https://go.microsoft.com/fwlink/?linkid=852256)。

>[!Note]
>Microsoft Forms 通常可供 Office 365 教育版客戶、Microsoft 365 Apps 商務版客戶，以及擁有 Microsoft 帳戶 (Hotmail、Live 或 Outlook.com) 的客戶使用。

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="預覽 Forms 在行動裝置上呈現的樣子。":::

## <a name="configure"></a>設定

Microsoft 365 系統管理員可以透過下列工作來控制 Microsoft Forms 在組織中的使用方式：

|系統管理員工作   |描述   |
|----------|-----------|
|**關閉或開啟 Microsoft Forms**|貴組織的 Microsoft Forms 預設為開啟。 您可以隨時 [將它關閉](turn-off-turn-on-microsoft-forms.md)。|
|**針對貴組織中的個別人員關閉 Microsoft Forms**|當您關閉特定人員的 Microsoft Forms 時，他們將無法使用 Microsoft Forms，而且 *Forms* 圖格也不會顯示在 Microsoft 365 應用程式啟動器或首頁中。 了解如何 [關閉特定人員的表單](turn-off-turn-on-microsoft-forms.md)。|
|**設定適用於 Microsoft Forms 的 Azure Active Directory 條件式存取**|若要設定 Microsoft Forms 的條件式存取原則，請參閱 [Azure AD 條件式存取文件](/azure/active-directory/conditional-access)，並在 *雲端應用程式* 指派中包含 *Microsoft Forms*。 <br/><br/> **注意：** 如果貴組織中的使用者在您設定 Microsoft Forms 的條件式存取之後仍遭到封鎖，請確定 SharePoint Online 和 Exchange Online 也透過條件式存取獲得存取權。 [深入了解](/azure/active-directory/conditional-access/block-legacy-authentication)。|
|**控制外部共用設定、記錄貴組織中人員的名稱，和/或保護表單不受網路釣魚的攻擊**|在 Microsoft 365 系統管理中心，您可以： <ul><li>控制是否允許外部使用者與貴組織中的使用者在表單或測驗上共同作業。</li><li>選擇是否要擷取貴組織中填寫表單的人員名稱。</li><li>關閉或開啟表單上的自動化網路釣魚偵測。</li></ul><br/>深入了解這些 [系統管理員設定](administrator-settings-microsoft-forms.md)。|
|**讓使用者可以將表單插入 PowerPoint**|<ol><li>登入https://admin.microsoft.com。</li><li>按一下 **[設定]**  >  **[設定]**。</li><li>在 **[設定]** 頁面上的 **[服務]** 索引標籤底下，按一下 **使用者擁有的應用程式和服務**。</li><li>請勾選此選項，**讓使用者存取 Office 市集**，允許使用者將表單插入 PowerPoint 中。</li></ol><br/>變更可能需要數小時，才會生效。 [深入了解](/microsoft-365/admin/manage/manage-deployment-of-add-ins)|

## <a name="security--compliance"></a>安全性與合規性

如果您的企業具有須符合內容安全性和資料使用的法律、法規和技術標準，推薦您參閱本節。

**Microsoft Forms 的資料儲存在哪裡？**

Microsoft Forms 資料儲存在美國和歐洲的伺服器上。 所有資料都位於美國，但在 2017 年 5 月之後開始使用 Microsoft Forms 的歐洲租用戶除外。 歐洲租用戶的資料儲存在歐洲的資料庫中。

**Microsoft Forms 是否符合規範？**

截至 2018 年 5 月，Microsoft Forms 已符合 GDPR 合規性要求。 如需詳細資訊，請前往 [[適用於 GDPR 的 Microsoft365 資料主體要求]](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json)。

**FERPA 和 BAA 防護是否就位？**

Microsoft Forms 符合 [FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) 和 [BAA 保護標準](https://www.microsoft.com/TrustCenter/Compliance/HIPAA)。

**即使使用者已離開組織，使用者數目和使用者帳戶所儲存的資料量是否都有限制？**

目前，保留資料的使用者數目沒有任何限制，只要其帳戶的佈建是在您組織的線上服務合約內。 使用者帳戶所儲存的資料量也沒有任何限制。

**表單的原始擁有者已不在我的組織中，且/或者已移除他們的 Microsoft Forms 授權。與其建立的表單相關聯之資料會發生什麼情況？**

從您的租用戶 (Azure AD) 刪除使用者帳戶的 30 天後，所有與帳戶相關的資料將會遭到刪除。

## <a name="faq"></a>常見問題集

**我可以使用 Microsoft Forms 做什麼？**

Microsoft Forms 是一款簡單、輕量的應用程式，可讓您輕鬆建立問卷、測驗及投票。 在教育機構中，它可以用來建立測驗、收集教師和父母的意見反應，或規劃班級和教職員活動。 在商務組織中，它可以用來收集客戶意見、衡量員工滿意度、改善您的產品或商務，或組織公司活動。

**誰可使用 Microsoft Forms？**

凡是擁有 Microsoft 帳戶 (Hotmail、Live 或 Outlook.com) 的使用者，就能免費使用 Microsoft Forms。 下列 Office 365 教育版和 Microsoft 365 Apps 商務版客戶也可以使用 Microsoft Forms：

**Office 365 教育版**

  - Office 365 A1 增強版

  - Office 365 A5

  - 在 Office 365 教育版 E3 停用之前購買的現有客戶

**Microsoft 365 Apps 商務版**

  - Microsoft 365 商務基本版

  - Microsoft 365 商務標準版

  - Microsoft 365 商務進階版

  - Microsoft 365 Apps 企業版

  - Microsoft 365 企業版 E1、E3 及 E5 方案

  - 在 E4 停用之前購買 E4 的現有 Office 365 企業版 E4 客戶

登入 [forms.office.com](https://forms.office.com/)，並開始建立問卷、測驗及投票。

**沒有 Microsoft 365 帳戶的人員是否仍可在 Microsoft Forms 上提交問卷或測驗？**

Microsoft Forms 作者可以切換其設定，以允許其組織外部的使用者回應其問卷或測驗。 在此情況下，使用者會匿名提交回應。 如果您想要查看已填寫問卷或測驗的人員，您可以要求回應者填入其名稱以作為問卷的一部分。

**可以建立的表單數目，以及表單可以接收的回應數目有什麼樣的限制？**

Office 365 教育版和 Microsoft 365 Apps 商務版客戶可以建立最多 200 個表單，而且每個表單最多可以接收 50,000 個回應。 具有 Microsoft 帳戶 (Hotmail、Live 或 Outlook.com) 的 Microsoft Forms 使用者可以建立最多 200 個表單，而且每個表單可接收最多 1,000 個付費帳戶的回應，以及最多 200 個免費帳戶的回應。 深入了解 [ Forms 中的表單、問題、回應及字元限制](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea)。

如果您需要更多回應，建議將現有的回應匯出至 Excel 活頁簿，然後清除問卷或測驗中的回應。 這可讓您在清除之後收集更多回應。

**Microsoft Forms 會使用哪些網頁瀏覽器？**

Microsoft Forms 已針對 Internet Explorer 11、Edge、Chrome (最新版本)、Firefox (最新版本)、Android 版 Chrome (最新版本) 以及 iOS 版 Safari (最新版本) 進行最佳化。

**Microsoft Forms 提供哪些語言？**

請參閱 Microsoft Forms 的 [支援的語言](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac) 和 [語言設定](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27)。

**Microsoft Forms 會取代 Microsoft InfoPath 嗎？**

錯誤。 Microsoft InfoPath 是一種解決方案，可建立啟用自動化工作流程的自訂表單，而 Microsoft Forms 是基本的輕量應用程式，用於透過問卷和測驗快速收集資訊。

Microsoft InfoPath 即將由 SharePoint 清單、Flow 和 PowerApps 取代 - 適用於數位化傳統公司表單、自動化工作流程並轉換商務程序的現代化解決方案。 [深入了解](https://products.office.com/business/business-process-automation)。

**哪裡可以提交意見反應，例如產品錯誤或功能要求？**

我們想知道您的想法！ 若要傳送有關 Microsoft Forms 的意見反應，請移至表單的右上角，然後選取 **[其他表單設定]** ![[其他選項] 按鈕](./media/image2.png)  >  **[意見反應]**。

> [!Note]
> 請參閱 [Microsoft Forms 的常見問題集](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c) 以深入了解。

