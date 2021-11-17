---
title: 檢閱和解除封鎖針對潛在網路釣魚進行偵測且遭到封鎖的表單或使用者
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft Forms 啟用自動化電腦檢閱，以主動偵測表單和問卷中的惡意敏感性資料收集。 如果您是全域和/或安全性系統管理員，您可以登入 Microsoft 365 系統管理中心，以檢視並解除封鎖針對潛在網路釣魚和惡意意圖進行偵測且遭到封鎖的表單。
ms.openlocfilehash: dd4b92c09393db4c81ac5e7711ee7331ac35558e
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951440"
---
# <a name="review-and-unblock-forms-or-users-detected-and-blocked-for-potential-phishing"></a>檢閱和解除封鎖針對潛在網路釣魚進行偵測且遭到封鎖的表單或使用者

Microsoft Forms 會啟用自動化電腦檢閱以主動偵測表單中惡意的敏感性資料收集，並暫時禁止這些表單收集回應。 深入了解 [Microsoft Forms 和主動式網路釣魚防護](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90)。

>[!Note]
>本文件中的步驟也適用於 [Dynamics 365 客戶語音](https://go.microsoft.com/fwlink/p?linkid=2128500) (以前稱為 Forms Pro)。 請注意，為了解除封鎖 Dynamics 365 客戶語音調查，需有 Dynamics 365 客戶語音授權。 [深入了解](/dynamics365/customer-voice/help-hub)。

## <a name="review-alerts-in-the-microsoft-365-defender-portal"></a>檢視 Microsoft 365 Defender 入口網站中的警示。

如果您是全域或安全性系統管理員，您會在 [Microsoft 365 Defender](https://security.microsoft.com/) 入口網站中收到有關您可以採取動作之潛在網路釣魚表單的警示。

>[!Note]
> 如果您是全域系統管理員，您會收到貴組織的資料隱私權訊息，包括您的租用戶中所建立之任何表單的每日通知 (針對潛在網路釣魚進行偵測並遭到封鎖的表單)。 您可以尋找 **Microsoft Forms 網路釣魚通知**，在 [[訊息中心]](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) 查看這些通知。 (如果您未在 **所有作用中訊息** 索引標籤/檢視中看到此通知，您可能會在 **關閉的訊息** 索引標籤/檢視中找到此訊息。) 針對每一則通知，請選取 **Forms 系統管理員檢閱 URL** 連結以檢閱遭封鎖的表單。  
  
為了讓安全性系統管理員也收到有關潛在網路釣魚表單的通知，全域系統管理員必須將 [[訊息中心] 隱私權讀取者](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) 角色指派給他們。 若要深入了解 [訊息中心]，請參閱 [常見問題](/microsoft-365/admin/manage/message-center)。 另請參閱如何 [設定資料隱私權訊息的電子郵件喜好設定](/microsoft-365/admin/manage/message-center#preferences)。

1.  登入 [Microsoft 365 Defender](https://security.microsoft.com/) 入口網站。

2.  選取 **事件和警示** \> **警示**。 您可能會看到其中一個或全部的下列 Forms 警示：
    
      - **限制使用者共用表單和收集回應**
    
      - **已標幟表單並確認為網路釣魚**
    
      - **表單因潛在網路釣魚嘗試而遭封鎖**

3.  選取警示以檢閱表單。 若要檢閱已標幟的表單，請點選或按一下 **管理警示** 按鈕旁邊右下角的三個點，然後選取 **檢閱此表單**。
 
    :::image type="content" source="./media/review-unblock-forms-review-this-form.png" alt-text="檢閱此表單選項":::

    >[!Tip]
    >深入了解 [Microsoft 365 中的警示原則](/microsoft-365/compliance/alert-policies)。

## <a name="unblock-a-form-or-confirm-its-phishing-attempt"></a>解除封鎖表單或確認其網路釣魚嘗試

針對您檢閱的每個表單，您可以選擇要對其解除封鎖或確認網路釣魚。

### <a name="unblock"></a>解除封鎖

如果您不認為表單具有惡意意圖，請選取 **解除封鎖**。

>[!Note]
>如果您租用戶中的某人要求您解除封鎖其表單，建議您要求特定表單資訊 (例如，遭封鎖的日期和時間、標題)，以便更有效地識別系統管理中心中的通知。 因為通知是每日傳送，並包含在過去 24 小時內偵測的所有表單，所以表單的可辨識資訊將會很實用。

### <a name="confirm-phishing"></a>確認網路釣魚

如果您認為表單具有惡意意圖，請選取 **確認網路釣魚**。 此表單會遭到永久封鎖，而且其擁有者將無法再對表單進行編輯或刪除。

當您選取了 **確認網路釣魚**，按一下或點選 **刪除表單**，以永久刪除租用戶中的表單。 我們強烈建議您立即針對您認為已遭入侵的租用戶帳戶進行密碼重設。

>[!Tip]
>您選擇的 **確認網路釣魚** 可協助 Microsoft Forms 改善其偵測準確度。 

## <a name="commonly-asked-questions"></a>常見問題

**當我檢閱遭封鎖的表單時，為何我看不到可解除封鎖或確認網路釣魚的選項？**

進行檢閱時，您可能會看到已解除的表單區塊。 這表示在表單遭到封鎖和您進行檢閱的時間之間，表單擁有者移除了已標幟為潛在網路釣魚的關鍵字。 在此案例中，您無須採取任何動作。

**如果表單因確認網路釣魚而遭封鎖，我可以將它移除嗎？**

如果表單已因確認網路釣魚而遭封鎖，請選取 **刪除表單** 以在您的租用戶中移除它。

**如果我對遭封鎖的表單未採取任何動作，該怎麼辦？**

如果您選擇不採取動作 (不解除封鎖表單或確認其網路釣魚意圖)，此表單會維持遭封鎖的狀態。 表單擁有者仍可編輯此表單，並移除已標幟為潛在網路釣魚的關鍵字。

**若要編輯或刪除表單中封鎖的內容，該怎麼辦？**

如果您想要編輯和/或刪除封鎖的內容，您可以共同作者來產生共同撰寫頁面並管理表單。 若要這麼做，在您正在檢閱的表單上方，按一下位於訊息中的 **開啟共同撰寫頁面** 連結。

## <a name="remove-restrictions-for-blocked-microsoft-forms-users"></a>移除已封鎖的 Microsoft Forms 使用者限制

Microsoft Forms 會禁止重複嘗試收集個人或敏感性資訊的使用者發佈表單和收集回應。 全域系統管理員會透過 [[訊息中心]](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) 收到這些使用者遭封鎖的通知。 如果您認為遭封鎖的使用者沒有惡意意圖，而且其帳戶是安全的，您可以採取下列步驟來解除封鎖。

>[!Note]
>當全域系統管理員將 [[訊息中心] 隱私權讀取者](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) 角色指派給使用者時，安全性系統管理員也可以收到有關潛在網路釣魚表單的通知。

1.  請移至 [[訊息中心]](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)，並尋找通知、**預防/修正：Microsoft Forms 偵測到的潛在網路釣魚**。

    >[!Note]
    >如果您未在 **所有作用中訊息** 索引標籤/檢視中看到此通知，您可能會在 **關閉的訊息** 索引標籤/檢視中找到此訊息。
 
    此通知包含您租用戶中的使用者清單，而這些使用者已遭到封鎖，無法共用表單及收集回應。

2.  按一下通知中提供的連結，以檢閱遭封鎖的使用者。

3.  對於您認為惡意意圖的每一位使用者，您可以選擇按一下與該使用者相關聯之 **[動作]** 欄中的 **解除封鎖** 連結。

    >[!Note]
    >如果您認為使用者具有惡意意圖，您不需要採取進一步的動作。

    >[!Note]
    >可能需要 30 分鐘以上的時間，才能移除限制。

