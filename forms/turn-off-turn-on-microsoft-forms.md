---
title: Microsoft Forms 끄기 또는 켜기
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: 이 문서에서는 Microsoft 365 관리자가 전체 조직 또는 조직의 특정 사용자에 대해 Microsoft Forms를 끄거나 켤 수 있는 방법을 설명합니다.
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951528"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>Microsoft Forms 끄기 또는 켜기

[Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8)는 기본적으로 조직의 모든 사용자에 대해 켜져 있습니다. [관리자](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504)인 경우 [Microsoft Forms를 설정](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240)한 다음 전체 조직 또는 특정 사용자에 대해 이 기능을 끄거나 다시 켤 수 있습니다.

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>조직의 모든 사용자에 대해 Microsoft Forms 끄기

1.  [Microsoft Azure](https://portal.azure.com/)에 로그인합니다.

2.  왼쪽 창에서 **Azure Active Directory**를 클릭합니다.

3.  **엔터프라이즈 애플리케이션**을 클릭합니다.

4.  필요한 서비스로 이동한 다음 **애플리케이션 유형**\> **CollabDBService** 및 **Microsoft 애플리케이션** \> **Microsoft Forms**에 대해 5-7단계를 반복합니다.
    
      - **애플리케이션 유형** 드롭다운 목록 아래의 검색 필드에 **CollabDBService**를 입력합니다. 검색 결과 목록에서 **CollabDBService**를 선택합니다.
    
      - **애플리케이션 유형** 드롭다운 목록에서 **Microsoft 애플리케이션**을 선택합니다. **애플리케이션 유형** 드롭다운 목록 아래의 검색 필드에 **Microsoft Forms**를 입력한 다음 검색 결과 목록에서 **Microsoft Forms**를 선택합니다.

5.  **관리**에서 **속성**을 클릭합니다.

6.  **사용자가 로그인할 수 있습니까?** 옵션에 대해 **아니요**를 선택합니다.

7.  **저장**을 클릭합니다.

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>조직의 특정 사용자에 대해 Microsoft Forms 끄기

1.  회사 또는 학교 계정을 전역 관리자로 사용하여 Microsoft 365에 로그인합니다. [로그인 방법에 대해 자세히 알아보세요](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4).

2.  Microsoft 365 관리 센터에서 **사용자** \> **활성 사용자**를 선택합니다.

3.  Microsoft Forms를 끄려는 사람의 이름 옆에 있는 상자를 선택합니다.

4.  리본에서 **제품 라이선스 관리**를 클릭합니다.

5.  열리는 계정 양식의 **라이선스 및 앱** 탭에서 앱 섹션을 확장하고 Microsoft Forms 옵션까지 아래로 스크롤합니다. 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Microsoft 365 관리 센터의 계정 옵션 양식":::

6.  Microsoft Forms를 끄려면 상자를 선택 취소합니다. 켜려면 확인란을 선택합니다.

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text=" Microsoft Forms 토글":::

     > [!Note]
     > [이 목록을 확인](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e)하여 Microsoft Forms가 포함된 Office 라이선스가 있는지 확인하세요. 라이선스가 목록에 있는 경우 사용자 액세스를 완전히 해제하려면 Microsoft Forms 확인란의 선택을 취소해야 합니다.

7.  **앱** 목록 하단에서 **변경 내용 저장**을 클릭합니다.

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>Microsoft Forms를 켰지만 조직의 사람들이 여전히 액세스할 수 없습니다.

Microsoft Azure에서 다음 설정을 확인하여 Microsoft Forms가 활성화되어 있는지 확인하세요.

1.  [Microsoft Azure](https://portal.azure.com/)에 로그인합니다.

2.  왼쪽 창에서 **Azure Active Directory**를 클릭합니다.

3.  **엔터프라이즈 애플리케이션**을 클릭합니다.

4.  필요한 서비스로 이동한 다음 **애플리케이션 유형**\> **CollabDBService** 및 **Microsoft 애플리케이션** \> **Microsoft Forms**에 대해 5-7단계를 반복합니다.
    
      - **애플리케이션 유형** 드롭다운 목록 아래의 검색 필드에 **CollabDBService**를 입력합니다. 검색 결과 목록에서 **CollabDBService**를 선택합니다.
    
      - **애플리케이션 유형** 드롭다운 목록에서 **Microsoft 애플리케이션**을 선택합니다. **애플리케이션 유형** 드롭다운 목록 아래의 검색 필드에 **Microsoft Forms**를 입력한 다음 검색 결과 목록에서 **Microsoft Forms**를 선택합니다.

5.  **관리**에서 **속성**을 클릭합니다.

6.  **사용자가 로그인할 수 있습니까?** 옵션에 대해 **예**를 선택합니다.

7.  **저장**을 클릭합니다.

    >[!Note]
    >조직의 사용자가 Microsoft Forms에 액세스할 수 있도록 SharePoint 서비스도 사용하도록 설정해야 합니다.

## <a name="feedback-for-microsoft-forms"></a>Microsoft Forms에 대한 피드백

의견을 보내 주세요.\! Microsoft Forms에 대한 의견을 보내려면 양식의 오른쪽 상단으로 이동하여 **추가 양식 설정** ![추가 옵션 버튼](./media/image2.png)\> **피드백**을 선택하세요.

