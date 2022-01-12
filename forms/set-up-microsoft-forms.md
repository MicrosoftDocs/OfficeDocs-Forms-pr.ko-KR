---
title: Microsoft Forms 설정
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: microsoft-365-education
ms.localizationpriority: high
description: Microsoft 365 관리자가 조직에서 Microsoft Forms 사용 방법을 제어하는 방법을 알아봅니다. 또한 Microsoft Forms용 데이터가 저장되는 위치와 같은 보안 및 규정 준수 질문에 대한 답변을 알아보세요.
ms.openlocfilehash: bb0e1a6ba8e2085550eb18a8bb393b34b197fe51
ms.sourcegitcommit: 80aa5565b4008855be844e8e5ab3f2779fba9a83
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/05/2022
ms.locfileid: "61723726"
---
# <a name="set-up-microsoft-forms"></a>Microsoft Forms 설정

## <a name="overview"></a>개요

Microsoft Forms를 사용하면 사용자 지정 퀴즈, 설문 조사, 선문지, 등록서 등을 쉽고 빠르게 만들 수 있습니다. 퀴즈 또는 설문지를 만들 때 모든 웹 브라우저를 사용하여 모바일 장치에서도 다른 사용자가 응답하도록 초대 할 수 있습니다. 결과가 제출되면 기본 제공 분석을 사용하여 응답을 평가할 수 있습니다. 퀴즈 결과와 같은 양식 데이터는 추가 분석이나 채점을 위해 Excel로 쉽게 내보낼 수 있습니다.

자세한 내용은 [Microsoft Forms란?](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8)을 참조하세요. 또는 Microsoft Forms에 대한 [Microsoft 365 블로그 게시물](https://go.microsoft.com/fwlink/?linkid=852256)을 참조하세요.

>[!Note]
>Microsoft Forms는 일반적으로 Office 365 Education 고객, 비즈니스용 Microsoft 365 앱 및 Microsoft 계정(Hotmail, Live 또는 Outlook.com)이 있는 고객에게 제공됩니다.

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="휴대용 장치에서 양식이 어떻게 보이는지에 대한 미리 보기.":::

## <a name="configure"></a>구성하기

Microsoft 365 관리자는 다음 작업을 통해 조직에서 Microsoft Forms를 사용하는 방법을 제어할 수 있습니다.

|관리자 작업   |설명   |
|----------|-----------|
|**Microsoft Forms 끄기 또는 켜기**|Microsoft Forms는 기본적으로 조직에 대해 켜져 있습니다. 언제든지 [해제](turn-off-turn-on-microsoft-forms.md)할 수 있습니다.|
|**조직의 개별 사용자에 대해 Microsoft Forms 끄기**|특정 사용자에 대해 Microsoft Forms를 끄면 해당 사용자는 Microsoft Forms를 사용할 수 없으며 *Forms* 타일이 Microsoft 365 앱 시작 관리자 또는 홈페이지에 표시되지 않습니다. [특정 사용자의 양식을 해제](turn-off-turn-on-microsoft-forms.md)하는 방법에 대해 알아보세요.|
|**Microsoft Forms에 대한 Azure Active Directory 조건부 액세스 설정**|Microsoft Forms에 대한 조건부 액세스 정책을 설정하려면 [Azure AD 조건부 액세스 문서](/azure/active-directory/conditional-access)를 참조하고 *클라우드 앱* 할당에 *Microsoft Form*을 포함하세요. <br/><br/> **참고: **Microsoft Forms에 대한 조건부 액세스를 설정한 후에도 조직의 사용자가 계속 차단되는 경우 SharePoint Online 및 Exchange Online에도 조건부 액세스를 통해 액세스 권한이 부여되었는지 확인하세요. [자세히 알아보기](/azure/active-directory/conditional-access/block-legacy-authentication).|
|**외부 공유 설정 제어, 조직 내 사람들의 이름 기록 및/또는 피싱으로부터 양식 보호**|Microsoft 365 관리 센터에서 다음을 수행할 수 있습니다. <ul><li>외부 사용자가 양식 또는 퀴즈에서 조직의 사용자와 공동 작업할 수 있는지 여부를 제어합니다.</li><li>조직에서 양식을 작성하는 사람의 이름을 캡처할지 여부를 선택합니다.</li><li>양식에서 자동 피싱 탐지를 끄거나 켭니다.</li></ul><br/>[관리자 설정](administrator-settings-microsoft-forms.md)에 대해 자세히 알아보세요.|
|**사용자가 PowerPoint에 양식을 삽입할 수 있도록 허용**|<ol><li>https://admin.microsoft.com에 로그인합니다.</li><li>**설정** > **설정**을 클릭합니다.</li><li>**설정** 페이지의 **서비스** 탭에서 **사용자 소유 앱 및 서비스**를 클릭합니다.</li><li>사용자가 PowerPoint에 양식을 삽입할 수 있도록 허용하려면 **사용자가 Office 스토어에 액세스하도록 허용** 옵션을 선택합니다.</li></ol><br/>변경 내용이 적용되는 데 몇 시간이 걸릴 수 있습니다. [자세한 정보](/microsoft-365/admin/manage/manage-deployment-of-add-ins)|

## <a name="security--compliance"></a>보안 및 규정 준수

비즈니스에 콘텐츠 보안 및 데이터 사용에 대해 충족해야 할 법적, 규제 및 기술 표준이 있는 경우 이 섹션이 적합합니다.

**Microsoft Forms용 데이터는 어디에 저장됩니까?**

Microsoft Forms 데이터는 미국과 유럽의 서버에 저장됩니다. 2017년 5월 이후에 Microsoft Forms를 사용하기 시작한 유럽 기반 테넌트를 제외한 모든 데이터는 미국에 있습니다. 그들의 데이터는 유럽의 데이터베이스에 저장됩니다.

**Microsoft Forms는 준수 요구 사항을 충족하나요?**

Microsoft Forms는 2018년 5월 현재 GDPR 준수 요구 사항을 충족했습니다. 자세한 내용을 확인하려면 [GDPR에 대한 Microsoft 365 데이터 주체 요청](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json)으로 이동하세요.

**FERPA 및 BAA 보호 조치가 마련되어 있나요?**

Microsoft Forms는 [FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) 및 [BAA 보호 표준](https://www.microsoft.com/TrustCenter/Compliance/HIPAA)을 충족합니다.

**사용자가 퇴사한 후에도 사용자 계정에 저장되는 데이터의 양과 사용자 수에 제한이 있나요?**

현재, 계정 프로비전이 조직의 온라인 서비스 계약 내에 있는 한 데이터가 보존되는 사용자 수에는 제한이 없습니다. 사용자 계정에 저장되는 데이터의 양에도 제한이 없습니다.

**양식의 원래 소유자가 더 이상 내 조직에 있지 않거나 Microsoft Forms 라이선스가 제거되었습니다. 해당 사용자들이 만든 양식과 연결된 데이터는 어떻게 되나요?**

모든 계정 관련 데이터는 사용자 계정이 테넌트(Azure AD)에서 삭제된 후 30일이 지나면 삭제됩니다.

## <a name="faq"></a>FAQ

**Microsoft Forms는 어떤 용도로 사용할 수 있나요?**

Microsoft Forms는 설문 조사, 퀴즈 및 투표를 쉽게 만들 수 있는 간단하고 가벼운 앱입니다. 교육 기관에서는 퀴즈를 만들고 교사와 학부모로부터 피드백을 수집하거나 수업 및 교직원 활동을 계획하는 데 사용할 수 있습니다. 비즈니스 조직에서는 고객 피드백을 수집하고, 직원 만족도를 측정하고, 제품이나 비즈니스를 개선하거나, 회사 이벤트를 조직하는 데 사용할 수 있습니다.

**누가 Microsoft Forms를 사용할 수 있나요?**

Microsoft Forms는 Microsoft 계정(Hotmail, Live 또는 Outlook.com)이 있다면 누구나 무료로 사용할 수 있습니다. 다음 Office 365 Education 및 기업용 Microsoft 365 앱 고객도 Microsoft Forms를 사용할 수 있습니다.

**Office 365 Education**

  - Office 365 A1 Plus

  - Office 365 A5

  - 사용 중지 전에 Office 365 Education E3를 구매한 기존 고객

**비즈니스용 Microsoft 365 앱**

  - Microsoft 365 Business Basic

  - Microsoft 365 Business Standard

  - Microsoft 365 Business Premium

  - 엔터프라이즈용 Microsoft 365 앱

  - Microsoft 365 Enterprise E1, E3 및 E5 플랜

  - E4가 만료되기 전에 구매한 기존 Office 365 Enterprise E4 고객

[forms.office.com](https://forms.office.com/)에 로그인하여 설문 조사, 퀴즈 및 투표를 만들기 시작하세요.

**Microsoft 365 계정이 없는 사람도 Microsoft Forms에서 설문 조사나 퀴즈를 제출할 수 있나요?**

Microsoft Forms 작성자는 조직 외부의 사용자가 설문 조사 또는 퀴즈에 응답할 수 있도록 설정을 전환할 수 있습니다. 이 경우 사용자는 익명으로 응답을 제출합니다. 설문 조사 또는 퀴즈를 작성한 사람을 확인하려면 응답자에게 설문지의 일부로 이름을 입력하도록 요구할 수 있습니다.

**만들 수 있는 양식의 수와 양식이 받을 수 있는 응답의 수에 대한 제한은 무엇인가요?**

Office 365 Education 및 비즈니스용 Microsoft 365 앱 고객은 최대 200개의 양식을 만들 수 있으며 각 양식은 최대 50,000개의 응답을 받을 수 있습니다. Microsoft 계정(Hotmail, Live 또는 Outlook.com)이 있는 Microsoft Forms 사용자는 최대 200개의 양식을 만들 수 있으며 각 양식은 유료 계정의 경우 최대 1,000개의 응답, 무료 계정의 경우 최대 200개의 응답을 받을 수 있습니다. [Forms 양식, 질문, 응답 및 문자 제한사항](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea)에 대해 자세히 알아보세요.

더 많은 응답이 필요한 경우 기존 응답을 Excel 통합 문서로 내보낸 다음 설문 조사나 퀴즈에서 지우는 것이 좋습니다. 이렇게 하면 삭제된 후에 더 많은 응답을 수집할 수 있습니다.

**Microsoft Forms는 어떤 웹 브라우저에서 작동하나요?**

Microsoft Forms는 Internet Explorer 11, Edge, Chrome(최신 버전), Firefox(최신 버전), Android의 Chrome(최신 버전), iOS의 Safari(최신 버전)에 최적화되어 있습니다.

**Microsoft Forms는 어떤 언어로 제공되나요?**

Microsoft Forms의 [지원되는 언어](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac) 및 [언어 설정](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27)을 참조하세요.

**Microsoft Forms가 Microsoft InfoPath를 대체하나요?**

아니요. Microsoft InfoPath는 자동화된 워크플로를 활성화할 수 있는 사용자 지정 가능한 양식을 만드는 솔루션인 반면 Microsoft Forms는 설문 조사와 퀴즈를 통해 정보를 빠르게 수집하기 위한 기본적이고 가벼운 앱입니다.

Microsoft InfoPath는 기존 회사 양식을 디지털화하고 워크플로를 자동화하며 비즈니스 프로세스를 변환하기 위한 최신 솔루션인 SharePoint 목록, Flow 및 PowerApps로 대체되고 있습니다. [자세히 알아보기](https://products.office.com/business/business-process-automation).

**어디서 제품 버그 또는 기능 요청과 같은 피드백을 제출할 수 있습니까?**

의견을 보내 주세요.  Microsoft Forms에 대한 의견을 보내려면 양식의 오른쪽 상단으로 이동하여 **추가 양식 설정** ![추가 옵션 버튼](./media/image2.png) > **피드백**을 선택하세요.

> [!Note]
> 자세한 내용은 [Microsoft Forms에 대해 자주 묻는 질문](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c)을 참조하세요.

