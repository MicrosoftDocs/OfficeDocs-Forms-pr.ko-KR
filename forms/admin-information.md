---
title: 관리자 정보
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 이 문서에서는 Microsoft Forms의 관리자 정보에 대해 가장 자주 묻는 질문에 대한 답변을 제공합니다.
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951565"
---
# <a name="admin-information"></a>관리자 정보

## <a name="getting-started"></a>시작하기

**Microsoft Forms를 끄거나 켜려면 어떻게 해야 하나요?**

기본적으로 Microsoft Forms는 조직의 모든 사용자에 대해 켜져 있습니다. Microsoft 365 IT 관리자는 Microsoft 365 관리 센터의 **사용자 관리** 탭에서 Microsoft Forms를 끌 수 있습니다. 자세한 내용은 [Microsoft Forms 설정](set-up-microsoft-forms.md) 및 [Microsoft Forms 끄기 또는 켜기](turn-off-turn-on-microsoft-forms.md)를 참조하세요.

**내 조직의 특정 사용자에게만 Microsoft Forms 액세스를 허용하려면 어떻게 해야 하나요?**

관리자는 조직의 특정 사용자에 대한 액세스 권한을 변경할 수 있습니다. [Microsoft Forms의 관리자 설정](administrator-settings-microsoft-forms.md)을 참조하세요.

## <a name="data-storage"></a>데이터 저장소

**Microsoft Forms용 데이터는 어디에 저장되나요?**

Microsoft Forms 데이터는 유럽 기반 테넌트에 대한 데이터를 제외하고 미국의 서버에 저장됩니다. 유럽 ​​기반 테넌트의 데이터는 유럽의 서버에 저장됩니다.

## <a name="user-activity"></a>사용자 활동

**내 조직의 사용자들이 Microsoft Forms에서 수행한 활동을 보려면 어떻게 해야 하나요?**

[Microsoft 365 보안 센터](https://security.microsoft.com/?rfr=OfficeScc) 감사 로그에서 [Microsoft Forms 활동](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities)을 검토할 수 있습니다. [Office 365에서 감사(관리자용)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906)에 대해 자세히 알아보세요.

## <a name="user-account-information"></a>사용자 계정 정보

**사용자 계정이 '완전 삭제'되었는지 확인하려면 어떻게 해야 하나요?**

1. 관리자는 [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer)에 로그인할 수 있습니다.

2. 상단 검색창에 다음 URL을 붙여넣습니다.

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*사용자 이메일* = 조직을 떠났거나 계정이 비활성화된 양식 소유자의 이메일 주소입니다.

3. **쿼리 실행**을 클릭합니다.

찾고 있는 계정 정보가 쿼리에 반환되면 계정이 일시 삭제되었으며 30일 제한 내에 있음을 의미합니다. 전역 관리자는 이전에 설명한 전송 방법을 사용하여 일시 삭제된 계정이 소유한 양식을 전송할 수 있습니다.

찾고 있는 계정 정보가 쿼리에 반환되지 않으면 계정이 Office 365 테넌트에 여전히 존재하거나 30일 이상 전에 삭제되었음을 의미합니다. 계정이 Office 365 테넌트에 존재하거나 비활성화된 상태인 경우 전역 관리자는 계정이 소유한 양식을 전송할 수 있습니다. 계정이 Office 365 테넌트에서 "완전 삭제"된 경우 전역 관리자는 해당 계정이 소유한 양식을 전송할 수 없습니다. 이러한 양식도 복구할 수 없습니다.

**사용자가 퇴사한 후에도 사용자 계정에 저장되는 데이터의 양과 사용자 수에 제한이 있나요?**

현재, 계정 프로비전이 조직의 온라인 서비스 계약 내에 있는 한 데이터가 보존되는 사용자 수에는 제한이 없습니다. 사용자 계정에 저장되는 데이터의 양에도 제한이 없습니다.

**소유자의 Microsoft Forms 라이선스가 제거되었거나 사용자가 테넌트(Azure AD)에서 비활성화 또는 삭제된 경우 양식 데이터는 어떻게 되나요?**

소유자 라이선스가 제거되었거나 소유자 계정이 비활성화된 경우 사용자 계정에 저장된 데이터 양에는 변경 사항이 없습니다.

테넌트(Azure AD)에서 사용자 계정이 삭제된 경우 사용자가 삭제된 후 30일이 지나면 모든 계정 관련 데이터가 삭제됩니다.

## <a name="form-ownership-transfer"></a>양식 소유권 이전

**양식의 원래 소유자가 더 이상 내 조직에 없습니다. 양식의 소유권을 이전하려면 어떻게 해야 하나요?**

퇴사한 사람의 양식을 이전하려면 다음 요구 사항이 충족되어야 합니다.

  - 귀하는 조직의 전역 관리자이며 유효한 Forms 라이선스가 있습니다.

  - 이전하려는 양식의 직원에게 삭제되거나 비활성화된 계정이 있습니다.

  - 양식은 계정이 삭제된 후 30일 이내에 이전됩니다.

> [!Note]
> 비활성화된(삭제되지 않은) 계정에서 양식의 소유권을 이전하는 데에는 시간 제한이 없습니다.

1. 모든 요구 사항이 충족되면 양식 소유권을 이전할 수 있습니다. 브라우저의 주소 표시줄에서 기존 URL을 다음으로 바꿉니다.

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*사용자 이메일* = 조직을 떠났거나 계정이 비활성화된 양식 소유자의 이메일 주소입니다.
   > 예를 들어 양식 소유자("Jason Fabian")가 조직("Contoso")을 떠난 경우 해결 방법 URL은 다음과 같습니다. `https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. 이제 이전 직원의 양식에 액세스할 수 있습니다. 전송할 양식에서 **추가 양식 작업**![추가 옵션 버튼](./media/image2.png)을 클릭한 다음 **이동**을 선택합니다.

   >[!Note]
   >현재 조직 내에서 활동 중인 직원에게 양식 소유권을 이전하려는 경우 해당 직원이 속한 그룹으로 양식을 이동할 수 있습니다. 아직 해당 그룹의 구성원이 아닌 경우 이전을 수행하려면 해당 그룹에 가입해야 합니다. 양식 소유권 이전이 완료된 후 그룹을 나가도록 선택할 수 있습니다.

**양식의 소유권을 이전하려고 할 때 오류가 발생하는 이유는 무엇인가요?**

오류 메시지가 표시되면 다음 중 하나가 소유권 이전을 방해할 수 있습니다.

|오류 메시지|설명|
| --- | --- |
| ***이 페이지에 액세스할 수 없습니다***<br/><br/>양식&#39;s 소유자는 여전히 활성 계정을 가지고 있습니다. | 양식 소유자는 여전히 활성 Forms 라이선스와 계정을 가지고 있습니다. |
| ***이 페이지에 액세스할 수 없습니다***<br/><br/>이메일 주소를 올바르게 입력했는지 확인하고&#39; 양식 소유자 계정이&#39; 30일 이상 전에 삭제되지 않았는지 확인하세요. | 이메일 주소의 철자가 잘못되었거나 양식 소유자의 계정이 30일 이상 전에 삭제되었습니다. |
| ***이 페이지에 액세스할 수 없습니다***<br/><br/>이메일 주소를&#39; 올바르게 입력했는지 확인한 다음 다시 시도하세요. | 이메일 주소가 누락되었거나 철자가 잘못되었습니다. |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Outlook 또는 PowerPoint에서 양식 사용

**내 조직의 사용자가 Outlook 이메일 메시지에 설문조사를 추가할 수 없습니다. 이 문제를 해결하려면 어떻게 해야 하나요?**

조직의 사용자가 [Outlook에서 설문 조사를 생성](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0)할 수 있도록 하려면 Outlook에 대한 **최신 인증** 설정을 활성화해야 합니다.

1. 회사 또는 학교 계정으로 [https://admin.microsoft.com](https://admin.microsoft.com/)에 로그인합니다.

2. **설정** \> **조직 설정**을 선택합니다.

   >[!Note]
   > **설정** 옵션이 표시되지 않으면 왼쪽 창에서 ![옵션 더보기 버튼](./media/image2.png)**모두 표시**를 선택합니다.

3.  **최신 인증**을 선택합니다.

4.  **Windows용 Outlook 2013 이상(권장)** 에 대한 최신 인증 켜기 옵션을 선택합니다.

최신 및 [다단계 인증](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide)과 설정 및 조직에 배포하는 방법에 대해 자세히 알아보세요.

**전체 조직에 Office 추가 기능을 배포하고 싶지 않습니다. 내 조직의 사용자가 PowerPoint용 Forms 추가 기능을 계속 사용할 수 있나요?**

예, [중앙 집중식 배포](/office/dev/add-ins/publish/centralized-deployment)를 사용하여 PowerPoint용 Forms 추가 기능만 배포할 수 있습니다.

1.  회사 또는 학교 계정으로 [https://admin.microsoft.com](https://admin.microsoft.com/)에 로그인합니다.

2.  **설정** \> **추가 기능**을 선택합니다.

    >[!Note]
    >**설정** 옵션이 표시되지 않으면 왼쪽 창에서 ![옵션 더보기 버튼](./media/image2.png)**모두 표시**를 선택합니다.

3.  **추가 기능** 목록에서 **양식**을 선택합니다.

4.  **양식 편집** 창의 **사용자 할당**에서 **모두**를 선택합니다.

5.  **저장**을 선택합니다.


## <a name="forms-and-anti-phishing"></a>양식 및 피싱 방지

**테넌트 내의 양식에 있는 피싱 및 잠재적인 악의적 의도에 대해 어떻게 해야 하나요?**

Microsoft Forms에서는 자동화된 시스템 검토를 통해 양식에서 중요한 데이터의 악의적인 수집을 사전에 검색하고 해당 양식이 응답을 수집하지 못하도록 일시적으로 차단합니다.

[Microsoft Forms 및 사전 예방적 피싱 방지](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90)에 대해 자세히 알아보세요.

전역 및/또는 보안 관리자인 경우 [admin.microsoft.com](https://admin.microsoft.com/)에서 Microsoft 365 관리 센터에 로그인하고 [메시지 센터](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)로 이동할 수 있습니다. 여기에서 차단된 모든 양식에 대한 일일 요약을 볼 수 있습니다. 나열된 각 양식에 대해 차단을 해제할지 또는 피싱 시도를 확인할지 선택할 수 있습니다. [잠재적인 피싱으로 검색 및 차단된 양식 또는 사용자를 검토 및 차단 해제](review-unblock-forms-users-detected-blocked-potential-phishing.md)하는 방법에 대해 자세히 알아보세요.
