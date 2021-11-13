---
title: 系統管理資訊
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 本文將回答最常見的 Microsoft 表單系統管理資訊常見問題集。
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951432"
---
# <a name="admin-information"></a>系統管理資訊

## <a name="getting-started"></a>開始使用

**如何關閉或開啟 Microsoft Forms？**

根據預設，會為組織中的每個人開啟 Microsoft Forms。 Microsoft 365 IT 管理員可以在 Microsoft 365 系統管理中心的 [**使用者管理**] 索引標籤下，關閉 Microsoft Forms。如需詳細資訊，請參閱[設定 Microsoft Forms](set-up-microsoft-forms.md) 和[關閉或開啟 Microsoft Forms](turn-off-turn-on-microsoft-forms.md)。

**如何只對組織中的特定人員允許 Microsoft Forms 存取權？**

系統管理員可以變更組織中特定人員的存取權限。 請參閱 [Microsoft Forms 中的系統管理員設定](administrator-settings-microsoft-forms.md)。

## <a name="data-storage"></a>資料儲存

**Microsoft Forms 的資料儲存在哪裡？**

Microsoft Forms 資料儲存在美國的伺服器上，但是歐洲租用戶的資料除外。 歐洲租用戶的資料會儲存在歐洲的伺服器上。

## <a name="user-activity"></a>使用者活動

**如何查看組織中的人員在 Microsoft Forms 中所執行的活動？**

您可以在 [Microsoft 365 安全性中心](https://security.microsoft.com/?rfr=OfficeScc)稽核記錄中查看 [Microsoft Forms 活動](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities)。 深入了解 [Office 365 中的稽核 (適用於系統管理員)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906)。

## <a name="user-account-information"></a>使用者帳戶資訊

**如何檢查使用者帳戶是否已「實刪除」？**

1. 系統管理員可以登入 [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer)。

2. 在頂端搜尋方塊中，貼上下列 URL：

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*使用者電子郵件* = 已經離開您的組織和/或其帳戶已停用之表單擁有者的電子郵件地址。

3. 按一下 [**執行查詢**]。

如果您要尋找的帳戶資訊在查詢中傳回，這表示該帳戶已虛刪除，且在 30 天的限制內。 全域系統管理員可以使用先前所述的傳輸方式，傳輸虛刪除帳戶所擁有的表單。

如果您要尋找的帳戶資訊未在查詢中傳回，這表示該帳戶仍存在於 Office 365 租用戶或是在 30 天前即已刪除。 如果帳戶存在於 Office 365 租用戶中或處於停用狀態，全域系統管理員可以傳輸該帳戶所擁有的表單。 如果帳戶從 Office 365 租用戶「實刪除」，全域系統管理員無法傳輸該帳戶所擁有的表單。 這些表單也無法復原。

**即使使用者已離開組織，使用者數目和為使用者帳戶儲存的資料量是否都有限制？**

目前，保留資料的使用者數目沒有任何限制，只要其帳戶的佈建是在您組織的線上服務合約內。 為使用者帳戶所儲存的資料量，也沒有任何限制。

**如果已移除擁有者的 Microsoft Forms 授權，或已從您的租用戶 (Azure AD) 停用或刪除使用者，表單的資料會發生什麼事？**

如果已移除擁有者授權，或擁有者的帳戶停用，則為使用者帳戶所儲存的資料量沒有任何變更。

如果已從您的租用戶 (Azure AD) 刪除使用者帳戶，則在刪除使用者 30 天之後，將會刪除所有與帳戶相關的資料。

## <a name="form-ownership-transfer"></a>表單擁有權轉移

**表單的原始擁有者已不會再與我的組織一起使用。如何轉移其表單的擁有權？**

若要轉移已離開組織之人員的表單，必須符合下列需求：

  - 您是組織的全域系統管理員，且具有有效的表單授權。

  - 您要轉移表單的員工其帳戶已刪除或停用。

  - 在刪除帳戶的 30 天內，會轉移表單。

> [!Note]
> 從已停用 (但未刪除) 的帳戶轉移表單的擁有權沒有時間限制。

1. 如果符合所有需求，您可以轉移表單擁有權。 在瀏覽器的位址列中，將現有 URL 取代為下列項目：

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*使用者電子郵件* = 已經離開您的組織和/或其帳戶已停用之表單擁有者的電子郵件地址。
   > 例如，如果表單擁有者 ("Jason Fabian") 已離開您的組織 ("Contoso")，您的因應措施 URL 看起來如下所示：`https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. 您現在可以存取離職員工的表單。 在您要轉移的表單上，按一下 [**其他表單動作**![更多選項] 按鈕](./media/image2.png)，然後選取 [**移動**]。

   >[!Note]
   >如果您嘗試將表單的擁有權轉移給組織中目前活躍的員工，您可以將其移至其所屬的群組。 如果您還不是該群組的成員，則必須加入該群組，才可以執行轉移。 在表單擁有權轉移完成之後，您可以選擇離開群組。

**當我嘗試轉移表單的擁有權時，為何會收到錯誤訊息？**

如果您收到錯誤訊息，下列任何一項可能會使您無法轉移擁有權：

|錯誤訊息|說明|
| --- | --- |
| ***我們無法存取此頁面***<br/><br/>表單的擁有者仍然具有使用中的帳戶。 | 表單的擁有者仍然具有使用中的表單授權和帳戶。 |
| ***我們無法存取此頁面***<br/><br/>請確認您輸入的電子郵件地址正確，且表單擁有者帳戶未在 30 天前刪除。 | 電子郵件地址拼寫錯誤，和/或表單擁有者的帳戶在 30 天前已刪除。 |
| ***我們無法存取此頁面***<br/><br/>請確認您輸入的電子郵件地址正確無誤，然後再試一次。 | 電子郵件地址遺失或拼錯。 |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Outlook 或 PowerPoint 中的表單使用狀況

**組織中的人員無法將投票新增至 Outlook 電子郵件訊息。如何修正此問題？**

必須啟用 Outlook 的**新式驗證**設定，以確保組織中的人員能夠[在 Outlook 中建立投票](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0)。

1. 使用您的公司或學校帳戶登入 [https://admin.microsoft.com](https://admin.microsoft.com/)。

2. 選取 [**設定** \> **組織設定**]。

   >[!Note]
   > 如果您看不到 [**設定**] 選項，請選取左窗格中的 [![其他選項按鈕](./media/image2.png)**全部顯示**]。

3.  選取 [**新式驗證**]。

4.  勾選選項，[**開啟 Outlook 2013 for Windows 及更新版本的新式驗證 (建議使用)**]。

深入了解新式和[多重要素驗證](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide)，以及如何設定並將其推出至您的組織。

**我不想在整個組織部署 Office 增益集。組織中的人員仍然可以使用 PowerPoint 的表單增益集嗎？**

是的，您可以使用 [[集中式部署](/office/dev/add-ins/publish/centralized-deployment)] 只部署 PowerPoint 的表單增益集。

1.  使用您的公司或學校帳戶登入 [https://admin.microsoft.com](https://admin.microsoft.com/)。

2.  選取 [**設定** \> **增益集**]。

    >[!Note]
    >如果您看不到 [**設定**] 選項，請選取左窗格中的 [![其他選項按鈕](./media/image2.png)**全部顯示**]。

3.  在 [**增益集**] 清單中，選取 [**表單**]。

4.  在 [**編輯表單**] 窗格的 [**指派使用者**] 下，選取 [**所有人**]。

5.  選取 [儲存]****。


## <a name="forms-and-anti-phishing"></a>表單和反網路釣魚

**我可以對租用戶內表單中的網路釣魚和潛在惡意意圖做什麼？**

在 Microsoft Forms 中，我們會啟用自動機器檢閱，以主動偵測出表單中惡意的敏感性資料集合，並且暫時封鎖這些表單免於收集回應。

深入了解 [Microsoft Forms 和主動式網路釣魚防護](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90)。

如果您是全球系統管理員和/或安全性管理員，您可以在 [admin.microsoft.com](https://admin.microsoft.com/) 登入 Microsoft 365 系統管理中心，並前往[訊息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)。 您可以在這裡看到任何和所有封鎖表單的每日摘要。 針對列出的每個表單，您可以選擇要解除封鎖或確認其網路釣魚企圖。 深入了解如何[檢閱和解除封鎖偵測到的表單或使用者，並封鎖潛在的網路釣魚](review-unblock-forms-users-detected-blocked-potential-phishing.md)。
