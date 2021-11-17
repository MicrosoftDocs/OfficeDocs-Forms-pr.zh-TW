---
title: Microsoft Forms 的系統管理員設定
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 本文涵蓋 Microsoft 365 系統管理員的 Microsoft Forms 設定。
ms.openlocfilehash: 371d3700a1d6157b3c65bc1b1b0224ef73f788a3
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951427"
---
# <a name="administrator-settings-for-microsoft-forms"></a>Microsoft Forms 的系統管理員設定

> [!Note]
> 系統管理員設定僅適用於 Office 365 教育版和Microsoft 365 Apps 商務版客戶。 若要存取這些設定，請使用您的公司或學校帳戶登入 [https://admin.microsoft.com](https://admin.microsoft.com/)。

## <a name="microsoft-365-admin-center"></a>Microsoft 365 系統管理中心

在 Microsoft 365 系統管理中心中，系統管理員可以控制外部共用設定、記錄組織中的人員名稱，和/或保護內部表單不受網路釣魚攻擊。

以下說明如何存取這些設定：

1.  使用您的公司或學校帳戶登入 [https://admin.microsoft.com](https://admin.microsoft.com/)。

2.  選取 **[設定]** \> **[組織設定]**。

    >[!Note]
    > 如果您看不到 **設定** 選項，請選取左窗格中的 ![其他選項按鈕](./media/image2.png) **全部顯示**。
 
3.  在 **[設定]** 頁面上，**[服務]** 索引標籤底下，按一下 **Microsoft Forms**。

請遵循下列步驟進行特殊設定。

### <a name="external-sharing"></a>外部共用

您可以控制是否允許外部使用者與貴組織中的使用者在表單或測驗上共同作業。 例如，您組織中的使用者建立表單，但想要：

  - 傳送表單連結至組織外部的人員，並收集外部人員的回應。

  - 與組織外部的人員共同處理表單 (例如，編輯問題、變更主題設計)。

  - 將表單共用為範本，讓組織外部的人員可以針對自己的用途來複製表單。

  - 與組織外部的人員共用表單結果的摘要。

>[!Tip]
>深入了解 [共用表單以進行共同作業](https://support.microsoft.com/office/share-a-form-or-quiz-to-collaborate-d5bb5cf0-8401-4c15-bb8c-8e108cd7e69b)。

若要控制 Microsoft 365 系統管理中心中的外部共用設定：

1.  在 **Microsoft Forms** 窗格上，**[外部共用]** 設定具有四個選項，預設會勾選所有選項。 取消核取您不想要的選項。

    :::image type="content" source="./media/admin-settings-external-sharing.png" alt-text="適用於外部共用的 Microsoft Forms 系統管理員設定":::

     >[!Note]
     >如果您想要讓組織中的使用者能夠 [在 Outlook 中建立投票](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0)，必須勾選 **傳送表單連結並收集回應** 選項。

2.  選取 **[儲存變更]**。

### <a name="record-names-of-people-in-your-org"></a>記錄貴組織中的人員名稱

您可以選擇是否要擷取表單回應者的名稱：

1.  在 **Microsoft Forms** 窗格上，系統會預設勾選 **紀錄貴組織中人員的名稱** 底下的 **[記錄名稱 (預設)]** 設定。 如果您不想要名稱與回應一起記錄，請取消勾選此選項。

    :::image type="content" source="./media/admin-settings-record-names.png" alt-text="適用於記錄名稱的 Microsoft Forms 系統管理員設定":::

1.  選取 **[儲存變更]**。

### <a name="phishing-protection"></a>網路釣魚防護

您可以針對網路釣魚偵測設定自動掃描組織內的表單：

1.  在 **Microsoft Forms** 窗格上，系統會預設勾選 **網路釣魚防護** 底下的 **內部網路釣魚防護** 設定。 如果您不想要網路釣魚掃描組織內的表單，請取消勾選此選項。

    :::image type="content" source="./media/admin-settings-phishing.png" alt-text="適用於網路釣魚防護的 Microsoft Forms 系統管理員設定":::

2.  選取 **[儲存變更]**。

### <a name="allow-youtube-and-bing"></a>允許 YouTube 和 Bing

您可以選擇是否允許組織中的人員從 Bing 新增影像，或將 YouTube 影片新增至問卷。

1.  在**Microsoft Forms**窗格上，系統預設會勾選 **允許 YouTube 和 Bing** 底下的 **包含 Bing 搜尋、YouTube 影片** 設定。 如果不想讓組織中的人員從 Bing.com 新增影像或從 YouTube.com 新增影片至表單，請取消勾選此選項。

    :::image type="content" source="./media/admin-settings-youtube-bing.png" alt-text="適用於 YouTube 和 Bing 的 Microsoft Forms 系統管理員設定":::

2.  選取 **[儲存變更]**。

### <a name="turn-off-or-turn-on-microsoft-forms-user-license-assignment"></a>關閉或開啟 Microsoft Forms 使用者授權指派

當您關閉使用者的 Microsoft 表單時，該人員無法使用 Microsoft Forms。 **Forms** 圖格將會隱藏在 Microsoft 365 應用程式啟動器和首頁中。 請查閱如何 [在 Microsoft 365 Apps 商務版中指派授權給使用者](https://support.microsoft.com/topic/997596b5-4173-4627-b915-36abac6786dc)，以取得關閉或開啟 Microsoft Form 個人版的步驟。

您也可以針對整個組織選擇 [關閉或開啟 Microsoft Forms](turn-off-turn-on-microsoft-forms.md)。
