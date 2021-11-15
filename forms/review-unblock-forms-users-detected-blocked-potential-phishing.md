---
title: 피싱 가능성이 있다고 검색되거나 차단된 양식 또는 사용자를 검토하고 차단을 해제합니다.
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft Forms를 사용하면 자동화된 시스템 검토를 통해 양식 및 설문 조사에서 악의적인 중요한 데이터 수집을 사전에 감지할 수 있습니다. 전역 및/또는 보안 관리자인 경우 Microsoft 365 관리 센터에 로그인하여 잠재적인 피싱 및 악의적인 의도로 검색 및 차단된 양식을 검토하고 차단 해제할 수 있습니다.
ms.openlocfilehash: dd4b92c09393db4c81ac5e7711ee7331ac35558e
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951581"
---
# <a name="review-and-unblock-forms-or-users-detected-and-blocked-for-potential-phishing"></a>피싱 가능성이 있다고 검색되거나 차단된 양식 또는 사용자를 검토하고 차단을 해제합니다.

Microsoft Forms를 사용하면 자동화된 시스템 검토를 통해 양식에서 중요한 데이터의 악의적인 수집을 사전에 검색하고 해당 양식이 응답을 수집하지 못하도록 일시적으로 차단합니다. [Microsoft Forms 및 사전 예방적 피싱 방지](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90)에 대해 자세히 알아보세요.

>[!Note]
>이 문서의 단계는 [Dynamics 365 Customer Voice](https://go.microsoft.com/fwlink/p?linkid=2128500)(이전 명칭: Forms Pro)에도 적용됩니다. Dynamics 365 Customer Voice 설문조사를 차단 해제하려면 Dynamics 365 Customer Voice 라이선스가 필요합니다. [자세히 알아보기](/dynamics365/customer-voice/help-hub).

## <a name="review-alerts-in-the-microsoft-365-defender-portal"></a>Microsoft 365 Defender 포털에서 경고 검토

전역 또는 보안 관리자인 경우 조치를 취할 수 있는 잠재적인 피싱 양식에 대한 경고를 [Microsoft 365 Defender](https://security.microsoft.com/) 포털에서 받게 됩니다.

>[!Note]
> 전역 관리자인 경우 잠재적인 피싱에 대해 감지 및 차단된 테넌트 내에서 생성된 모든 양식에 대한 일일 알림을 포함하여 조직에 대한 데이터 개인 정보 보호 메시지를 받게 됩니다. **Microsoft Forms 피싱 알림**을 검색하면 [메시지 센터](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)에서 이러한 알림을 볼 수 있습니다. (**모든 활성 메시지** 탭/보기에 이 알림이 표시되지 않으면 **닫은 메시지** 탭/보기에서 찾을 수 있습니다.) 각 알림에 대해 **양식 관리자 검토 URL** 링크 또는 차단된 양식 검토 링크를 선택합니다.  
  
보안 관리자가 잠재적인 피싱 양식에 대한 알림도 수신하려면 전역 관리자가 [메시지 센터 개인 정보 보호 읽기 권한자](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) 역할을 할당해야 합니다. 메시지 센터에 대해 자세히 알아보려면 [자주 묻는 질문](/microsoft-365/admin/manage/message-center)을 참조하세요. 또한 [데이터 개인 정보 보호 메시지에 대한 이메일 환경 설정을 지정](/microsoft-365/admin/manage/message-center#preferences)하는 방법을 참조하세요.

1.  [Microsoft 365 Defender](https://security.microsoft.com/) 포털에 로그인합니다.

2.  **인시던트 및 경고** \> **경고**를 선택합니다. Forms에 대해 다음 경고 중 하나 또는 모두가 표시될 수 있습니다.
    
      - **양식 공유 및 응답 수집이 제한된 사용자**
    
      - **피싱으로 신고 및 확인된 양식**
    
      - **잠재적인 피싱 시도로 인해 차단된 양식**

3.  경고를 선택하여 검토하세요. 신고된 양식을 검토하려면 **r경고 관리** 버튼 옆의 오른쪽 하단 모서리에 있는 세 개의 점을 탭하거나 클릭한 다음 **이 양식 검토**를 선택합니다.
 
    :::image type="content" source="./media/review-unblock-forms-review-this-form.png" alt-text="이 양식 옵션 검토":::

    >[!Tip]
    >[Microsoft 365의 경고 정책](/microsoft-365/compliance/alert-policies)에 대해 자세히 알아보세요.

## <a name="unblock-a-form-or-confirm-its-phishing-attempt"></a>양식 차단 해제 또는 피싱 시도 확인

검토하는 각 양식에 대해 차단 해제 또는 피싱 확인 여부를 선택할 수 있습니다.

### <a name="unblock"></a>차단 해제

양식에 악의적인 의도가 있다고 생각되지 않으면 **차단 해제**를 선택합니다.

>[!Note]
>테넌트의 누군가가 양식 차단 해제를 요청하는 경우 관리 센터에서 알림을 보다 효율적으로 식별하기 위해 특정 양식 정보(예: 차단 날짜 및 시간, 제목)를 요청하는 것이 좋습니다. 알림은 매일 전송되고 지난 24시간 동안 감지된 모든 양식을 포함하므로 양식에 대한 식별 가능한 정보가 도움이 될 것입니다.

### <a name="confirm-phishing"></a>피싱 확인

양식에 악의적인 의도가 있다고 생각되면 **피싱 확인**을 선택합니다. 양식은 영구적으로 차단되며 소유자는 더 이상 양식을 편집하거나 삭제할 수 없습니다.

**피싱 확인**을 선택한 후 **양식 삭제**를 클릭하거나 탭하여 테넌트에서 양식을 영구적으로 삭제합니다. 손상되었다고 생각되는 테넌트의 계정에 대해 즉시 암호를 다시 설정하는 것이 좋습니다.

>[!Tip]
>**피싱 확인**을 선택하면 Microsoft Forms가 검색 정확도를 높이는 데 도움이 됩니다. 

## <a name="commonly-asked-questions"></a>자주 묻는 질문

**차단된 양식을 검토할 때 차단 해제 또는 피싱 확인 옵션이 표시되지 않는 이유는 무엇입니까?**

검토 시 양식에 대한 차단이 이미 해제된 것을 볼 수 있습니다. 이는 양식이 차단된 시간과 귀하가 양식을 검토한 시간 사이에 양식 소유자가 잠재적인 피싱으로 표시된 키워드를 제거했음을 의미합니다. 이 시나리오에서는 추가 조치가 필요하지 않습니다.

**확인된 피싱으로 인해 양식이 차단된 경우 제거할 수 있나요?**

확인된 피싱에 대해 양식이 이미 차단된 경우 **양식 삭제**를 선택하여 테넌트에서 제거합니다.

**차단된 양식에 대해 아무 조치도 취하지 않으면 어떻게 되나요?**

조치를 취하지 않기로 선택하면(양식 차단 해제 또는 피싱 의도 확인) 양식이 차단된 상태로 유지됩니다. 양식 소유자는 여전히 양식을 편집하고 잠재적인 피싱으로 표시된 키워드를 제거할 수 있습니다.

**양식에서 차단된 콘텐츠를 편집하거나 삭제하려면 어떻게 하나요?**

차단된 콘텐츠를 편집 및/또는 삭제하려는 경우 공동 작성 페이지를 생성하고 양식을 공동 작성자로 관리할 수 있습니다. 이렇게 하려면 검토 중인 양식 위의 메시지에 있는 **공동 작성 페이지 열기** 링크를 클릭하세요.

## <a name="remove-restrictions-for-blocked-microsoft-forms-users"></a>차단된 Microsoft Forms 사용자에 대한 제한 제거

Microsoft Forms는 개인 정보 또는 중요한 정보 수집을 반복적으로 시도한 사용자가 양식 배포 및 응답 수집을 차단합니다. 전역 관리자는 [메시지 센터](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)를 통해 차단된 사용자에 대한 알림을 받게 됩니다. 차단된 사용자가 악의적인 의도를 나타내지 않고 계정이 안전하다고 생각되면 다음 단계에 따라 차단을 해제할 수 있습니다.

>[!Note]
>전역 관리자가 [메시지 센터 개인 정보 보호 읽기 권한자](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader) 역할을 할당하고 나면 보안 관리자는 잠재적인 피싱 양식에 대한 알림도 수신할 수 있습니다.

1.  [메시지 센터](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)로 이동하여 **방지/수정: Microsoft Forms가 잠재적인 피싱 감지** 알림을 찾습니다.

    >[!Note]
    >**모든 활성 메시지** 탭/보기에 이 알림이 표시되지 않으면 **닫은 메시지** 탭/보기에서 찾을 수 있습니다.
 
    이 알림에는 양식 공유 및 응답 수집이 차단된 테넌트의 사용자 목록이 포함되어 있습니다.

2.  차단된 사용자를 검토하려면 알림에 제공된 링크를 클릭하세요.

3.  악의적인 의도가 없다고 생각되는 각 사용자에 대해 해당 사용자와 연결된 **작업** 열에서 **차단 해제** 링크를 클릭하도록 선택할 수 있습니다.

    >[!Note]
    >사용자가 악의적인 의도를 가지고 있다고 생각되면 추가 조치가 필요하지 않습니다.

    >[!Note]
    >제한이 제거되기까지 30분 정도 걸릴 수 있습니다.

