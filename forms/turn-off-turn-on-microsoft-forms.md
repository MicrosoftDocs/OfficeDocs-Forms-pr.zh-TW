---
title: 關閉或開啟 Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 本文涵蓋 Microsoft 365 系統管理員如何針對整個組織或組織中的特定人員關閉或開啟 Microsoft Forms。
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951419"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>關閉或開啟 Microsoft Forms

根據預設，系統會為您組織中的每個人開啟 [Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8)。 如果您是 [系統管理員](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504)，您可以 [設定 Microsoft Forms](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240)，然後針對整個組織或僅特定人員將其關閉或再次開啟。

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>針對貴組織中的所有人關閉 Microsoft Forms

1.  登入至 [Microsoft Azure](https://portal.azure.com/)。

2.  在左側窗格中，按一下 **Azure Active Directory**。

3.  按一下 **企業應用程式**。

4.  瀏覽至必要的服務，然後針對 **應用程式類型** \> **CollabDBService** 和 **Microsoft 應用程式** \> **Microsoft Forms**，重複步驟 5-7。
    
      - 在 **應用程式類型** 下拉式清單底下的搜尋欄位中，輸入 **CollabDBService**。 在搜尋結果清單中選取 **CollabDBService**。
    
      - 在 **應用程式類型** 下拉式清單中，選取 **Microsoft 應用程式**。 在 **應用程式類型** 下拉式清單底下的搜尋欄位中，輸入 **Microsoft Forms**，然後在搜尋結果清單中選取 **Microsoft Forms**。

5.  在 [管理]**** 底下，按一下 [內容]****。

6.  針對 [為使用者啟用登入?]**** 選項，選取 [否]****。

7.  按一下 [儲存]****。

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>針對貴組織中特定人員關閉 Microsoft Forms

1.  使用您的公司或學校帳戶，以全域系統管理員的身分登入 Microsoft 365。[了解如何登入](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4)。

2.  在 Microsoft 365 系統管理中心中，選擇 **[使用者]** \> **[作用中使用者]**。

3.  選取您想要關閉 Microsoft Forms 之人員名稱旁的方塊。

4.  在功能區上，按一下 **管理產品授權**。

5.  在開啟的帳戶表單上，在 **授權與應用程式** 索引標籤上，展開 [應用程式] 區段並向下捲動至 Microsoft Forms 選項。 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Microsoft 365 系統管理中心中的 [帳戶選項] 表單":::

6.  清除此方塊以關閉 Microsoft Forms。 若要將其開啟，請選取核取方塊。

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text="Microsoft Forms 切換":::

     > [!Note]
     > [檢查此清單](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e)，查看您是否擁有包含 Microsoft Forms 的 Office 授權。 如果您的授權已列出，您就必須清除 Microsoft Forms 核取方塊，以完全關閉使用者存取。

7.  在 **應用程式** 清單底部，按一下 **[儲存變更]**。

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>我已開啟 Microsoft Forms，但組織中的人員仍無法存取它

檢查 Microsoft Azure 中的下列設定，確定已啟用 Microsoft Forms：

1.  登入至 [Microsoft Azure](https://portal.azure.com/)。

2.  在左側窗格中，按一下 **Azure Active Directory**。

3.  按一下 **企業應用程式**。

4.  瀏覽至必要的服務，然後針對 **應用程式類型** \> **CollabDBService** 和 **Microsoft 應用程式** \> **Microsoft Forms**，重複步驟 5-7。
    
      - 在 **應用程式類型** 下拉式清單底下的搜尋欄位中，輸入 **CollabDBService**。 在搜尋結果清單中選取 **CollabDBService**。
    
      - 在 **應用程式類型** 下拉式清單中，選取 **Microsoft 應用程式**。 在 **應用程式類型** 下拉式清單底下的搜尋欄位中，輸入 **Microsoft Forms**，然後在搜尋結果清單中選取 **Microsoft Forms**。

5.  在 [管理]**** 底下，按一下 [內容]****。

6.  針對 [為使用者啟用登入?]**** 選項，選取 [是]****。

7.  按一下 [儲存]****。

    >[!Note]
    >也必須啟用 SharePoint 服務，讓您組織中的人員可以存取 Microsoft Forms。

## <a name="feedback-for-microsoft-forms"></a>Microsoft Forms 的意見反應

我們想知道您的想法\! 若要傳送有關 Microsoft Forms 的意見反應，請移至表單的右上角，然後選取 **[其他表單設定]** ![[其他選項] 按鈕](./media/image2.png) \> **意見反應**。

