---
description: 오픈소스 공개를 위해 준비해야 할 사항들을 설명합니다.
---

# 준비 사항

기존의 오픈소스 프로젝트에 기여하기 위한 사항은 다음 페이지를 참고하세요. 

{% page-ref page="../../../contribute/main/" %}

SK텔레콤은 오픈소스를 통해 가치 창출을 기대하며 이를 지원합니다. SK텔레콤의 소프트웨어를 오픈소스로 공개하기 위한 승인을 요청하기 전에 다음의 사항들을 준비해야 합니다. 

## 프로젝트의 이름 정하기

프로젝트의 이름은 시장에서 일관된 메시지를 보장하는 데 도움이 되기 때문에 특히 중요합니다. 프로젝트가 무엇인지 나타내는데 도움이 되는 이름을 사용하는 것이 좋습니다. 이를 위해 다음 가이드를 따르세요. 

* 프로젝트가 무엇을 하는지를 설명할 수 있는 이름을 사용하세요.
* SK텔레콤이 홍보하는 제품 혹은 서비스가 아니라면 SK텔레콤의 브랜드를 사용하지 마세요.
  * 꼭 필요한 경우가 아니라면 "T-이름" 형태의 이름\(예: T world\)을 사용하지 마세요. 
* 타사 브랜드를 사용하지 마세요. 
  * 즉, "Java Test Library" 보다는 "Test Library for Java"가 낫습니다.

{% hint style="warning" %}
Repository 이름의 경우, 하이픈 \("-"\)으로 구분합니다. 

**DON'T** : successortoserverless  
**DO** : successor-to-serverless
{% endhint %}

## 프로젝트에 라이선스 부여하기

SK텔레콤은 오픈소스로 공개 시 기본적으로 [Apache-2.0](https://spdx.org/licenses/Apache-2.0.html)를 적용합니다. Apache-2.0는 사용자에게 광범위한 자유를 제공하면서 명시적인 특허 허여 조항 등 법적인 관점에서도 가장 적절한 라이선스입니다. 

만약, 다른 라이선스를 선택해야 할 상황이라면 오픈소스팀에 문의하시기 바랍니다. \(haksung : 문의 방법 추가 필요\)

{% hint style="warning" %}
오픈소스 공개 시 라이선스 선택에 대한 안내는 GitHub에서 제공하는 라이선스 선택 가이드를 참고할 수 있습니다. : [https://choosealicense.com](https://choosealicense.com)
{% endhint %}















### 법률 검토

#### \(1\) 출처 확인

오픈소스 프로젝트에서 발생할 수 있는 최악의 상황 중 하나는 법적으로 문제가 있는 코드가 포함되었다고 알려지는 것입니다. 따라서, 코드를 릴리즈하기 전에 출처를 명확히 확인하는 것이 중요합니다. 

* 법적 검토의 핵심은 회사가 모든 코드를 공개할 권리가 있는지 확인하는 것입니다. 
* 또 공개하려는 코드가 저작권, 특허 등 다른 회사의 IP를 침해하지 않도록 해야 합니다. 

이를 위해 Protex와 같은 검사 도구를 사용하여 문제가 없는지 확인할 수 있습니다. 

#### \(2\) 라이선스 선택

또한 오픈소스에 적용할 라이선스를 선택해야 합니다. 

일반적인 오픈소스 라이선스와 각각의 장단점에 대해 파악하고 있어야 합니다. 일반적으로는 Copyleft 성격의 라이선스와 Permissive 성격의 라이선스 중 선택합니다. 

* Copyleft 성격의 라이선스는 GPL이 대표적이며, 재배포 시, 수정 부분을 포함한 소스 코드의 공개를 요구합니다. 
* Permissive 성격의 라이선스는 이러한 소스 코드 공개 요구 사항이 없습니다. 따라서, 사용자가 변경 사항을 공개하지 않고 독점 소프트웨어를 배포할 수 있게 합니다. 
* 프로젝트에는 소스 코드 이외의 결과물이 포함될 수도 있습니다. 특히 문서를 제작하는 경우, 문서를 어떤 라이선스로 공개할지에 대해서도 고려가 필요합니다. 일반적으로 오픈소스 프로젝트는 문서를 공개할 때는 Creative Commons 라이선스를 사용합니다. 

라이선스 선택을 위한 자세한 사항은 다음 페이지를 참고하세요. 





#### \(3\) 저작권 및 라이선스 표기

라이선스를 선택했으면, 공개할 코드 내에 코드의 각 파일에 저작권과 라이선스를 표기해야 합니다. 이를 위한 세부 내용은 다음 페이지를 참고하세요. 







#### \(4\) Contributor Agreement

일반적인 오픈소스 라이선스는 기여자로부터의 라이선싱도 명시하고 있기 때문에 추가적인 Contributor Agreement가 필요하지 않습니다. 필요에 따라 코드의 법적 문제를 방지하기 위해 기여자에게 CLA \(Contributor License Agreement\)나 DCO\(Developer Certificate of Origin\)를 요구하는 것도 고려할 수 있습니다. CLA와 DCO에 대한 세부 내용은 다음 페이지를 참고하세요. 







### 기술 검토

공개하려는 소스 코드가 회사 내부 코드나 환경에 종속되지 않고 동작하는지 확인합니다. 또 모든 라이선스 및 저작권 고지에 대한 확인 및 불필요한 주석을 제거합니다. 주요 단계는 다음과 같습니다.

#### \(1\) Dependency 제거

공개하지 않아야 하는 소프트웨어와의 Dependency를 제거하세요. 

#### \(2\) 문서와 예제 제공

기술 문서와 Use Case 예제를 제공하세요. 문서의 가장 기본은 README 입니다. README 작성 방법은 다음 페이지를 참고하세요. 



#### \(3\) 불필요한 주석 제거

회사 내부 주석 및 내부 코드에 대한 Reference를 제거하세요.

#### \(4\) 코딩 스타일

코딩 스타일을 일관성 있게 유지하세요.

#### \(5\) 기여 방법 안내

기여하는 방법을 안내하세요. 자세한 사항은 다음 페이지를 참고하세요.







### 거버넌스 수립

거버넌스는 프로젝트가 전략, 릴리스, 방향 및 개발 우선순위에 관한 결정을 내리는 프로세스입니다. 

모든 참여자가 프로젝트의 변경 사항을 인식할 수 있도록 의사 결정은 공개적이고 투명해야 합니다. 거버넌스 기구에 참여하기 위해 충족해야 할 기준을 결정하고, 기능 및 버그 추적 방법, 코드 제출 방법 및 릴리스 프로세스 관리에 대한 결정 방법을 수립합니다.

거버넌스에 대한 자세한 내용은 다음 페이지를 참고하세요. 



### 리더쉽 역할 정의

프로젝트를 시작하기 전에 리더쉽 역할을 정하는 것도 중요합니다. 여러 기업 참가자와 함께 프로젝트를 시작하는 경우 프로젝트에는 관리 위원회 \(Governing Board\)와 같은 공식적인 거버넌스 조직이 필요할 수 있습니다.

리더쉽에 대한 자세한 내용은 다음 페이지를 참고하세요. 



### 인프라 구축

프로젝트를 위한 저장소를 준비하세요. 많은 프로젝트가 GitHub 또는 GitLab repository를 사용하거나 Gerrit과 같은 도구를 사용하여 자체 저장소를 제공합니다. 

* Bug, issue, feature tracking을 위한 기능도 인프라 계획의 일부로 포함되어야 합니다. 
* 사용자가 이슈 리포트 및 Feature Request를 쉽게 작성할 수 있는 장소를 제공해야 합니다.  
* 그리고, 빌드 자동화, Unit Test 환경을 구축하여 코드를 확인하여 품질을 보장해야 합니다. \(참고 : [https://blog.banksalad.com/tech/become-an-organization-that-deploys-1000-times-a-day/](https://blog.banksalad.com/tech/become-an-organization-that-deploys-1000-times-a-day/)\)

### 웹사이트 구축

다음 단계는 프로젝트를 위한 회사와 관계없는 중립적인 웹사이트 또는 위키 페이지를 개설하는 것입니다. 

웹페이지는 문서, 코드 다운로드 링크 등의 프로젝트에 대한 정보를 커뮤니티에 제공하기 위한 장소입니다. 또한, 웹사이트에서는 프로젝트의 리더쉽, 거버넌스 세부 사항 등에 대한 내용도 제공할 수 있습니다.

### 커뮤니케이션 채널 제공

커뮤니티에서 원활한 커뮤니케이션이 가능하도록 채널을 제공하는 것이 중요합니다. 또한 코드 체크인, 오류 로그 등 기타 작업에 대한 알림을 주는 등 전체 개발 Work Flow에 통합할 수 있는 도구가 필요합니다. 이는 프로젝트를 실시간으로 진행하는 중요한 수단이 됩니다. 

* 우수한 도구 중 하나는 [Slack](https://slack.com/)입니다. Slack은 사용자가 메시지와 파일을 공유하고, Work Flow 구성, 정보 검색 등의 작업을 수행할 수 있게 하는 온라인 프로젝트 관리 및 통신 플랫폼입니다. 그러나 Slack은 상용 도구이며 유지 관리 비용이 발생합니다. 
* 오픈소스로 공개된 도구들로는 IRC, [Gitter.im](https://gitter.im/), [Rocket.Chat ](https://rocket.chat/)등이 있습니다. Rocket.Chat은 오픈소스이며 Slack과 유사한 기능을 제공합니다. 

### 런칭

모든 준비와 검토 단계를 마친 후에는 최종적으로 다음 사항을 확인합니다. 

* 모든 프로젝트 인프라가 실행 중이고, 안전하며, 확장 가능한지 확인하세요.
* 개발자가 커뮤니케이션 채널 \(IRC, Mailing List 등\)에 참여하고 모니터링할 수 있는지 확인하세요. 

그리고, 오픈소스 프로젝트를 런칭합니다. 소스 코드를 저장소에 릴리즈하세요. 

이제, 오픈소스 개발 모델을 따라 프로젝트를 운영합니다. 

## 마케팅과 브랜딩

런칭이 단계의 마지막이 아닙니다. 프로젝트를 계속 진행하기 위해서는 마케팅 단계가 필수적입니다. 

마케팅에는 프로젝트 홍보, 성공적인 운영 전략 수립, 현실적인 예산 및 프로젝트 브랜딩 제공, 소셜 미디어 계정 활성화 등 장기적인 성공을 위한 활동 등이 포함됩니다. 일반적인 마케팅 검토 절차는 다음과 같습니다. 

1. 프로젝트 로고, Color Scheme, 웹사이트 등을 디자인하세요. 
2. 소셜 미디어 계정을 등록하세요. \(Twitter, Facebook, LinkedIn 등\)
3. Domain Name을 등록하세요.

또한 브랜딩에 대한 가이드라인을 만듭니다. 

브랜딩은 시장에서 일관된 메시지를 보장하는 데 도움이 되기 때문에 특히 중요합니다. 브랜딩에 대한 세부 내용은 다음 페이지를 참고하세요. 







오픈소스 프로젝트를 시작하기 전 고려해야 할 여러 사항이 있습니다. 

## 1. 비즈니스와 연계하세요.

일반적인 제품들과 같이, 오픈소스 프로젝트도 비즈니스 사례와 연계하여 준비하는 것이 좋습니다. 

왜 수행되어야 하는지, 목표와 예산은 무엇인지, 로드맵은 어떻게 구성할지, 어떤 지식 재산을 공개할 것인지, 어떤 코드가 공개 대상에 포함되는지에 대하여 경영진을 이해시킬 수 있어야 합니다.

## 2. 리소스를 준비하세요. 

개발자를  포함해서 프로젝트에 투입해야 하는 리소스를 할당해야 합니다. 

* 초기에는 일반적인 사내 프로젝트와 비슷한 수준의 개발자가 필요합니다. 
* 또한, 외부의 기여를 신속하게 리뷰 할 수 있도록 개발자 리소스가 필요함을 고려해야 합니다. 
* 그리고, 법무팀, 마케팅팀의 역할도 필요합니다. 
* 또한, 프로젝트를 유지, 관리하는데 요구되는 인프라에 대한 예산을 확보해야 합니다. 여기에는 Github와 같은 프로젝트 호스팅을 위한 도구가 포함됩니다.

## 3. 코드 품질을 확인하세요. 

코드의 가독성과 성숙도는 오픈소스로 공개하기 위한 준비가 되었는지에 대한 척도가 될 수 있습니다. 쓰레기 같은 코드는 커뮤니티의 신뢰를 잃게 합니다. 

그렇다고 코드가 완벽해야 한다는 건 아닙니다. 코드를 완벽하게 준비하려고 한다면 아마 시작할 수도 없을 것입니다. 주어진 환경에서 최선의 수준으로 준비하여 공개하세요. 다른 사람들이 개선하는 데 참여할 것입니다. 

대신, 공개하려는 코드에 회사의 영업 비밀이나 문제를 일으킬만한 불필요한 주석이 포함되지 않도록 확인하세요. 

## 4. 코드가 유용할까요?

성공적인 프로젝트가 되기 위해서는 다른 사람들에게도 유용해야 합니다. 

만약, 유사한 프로젝트가 이미 존재한다면, 새로운 프로젝트를 만드는 것보다 기존의 프로젝트에 참여하는 것도 고려할 수 있습니다. 경쟁 업체가 추진하는 프로젝트라도 오픈소스에서는 협력하는 것이 중요합니다. 함께 참여하고 협력하면서 모두가 훌륭한 코드를 가질 수 있습니다. 

단, 더 이상 유용하지 않은 코드인데도 공개만 하면 무조건 커뮤니티가 관리할 것으로 생각해서는 안 됩니다. 오픈소스 커뮤니티는 오래된 코드를 관리해주는 조직이 아닙니다. 실제로 매력적이지 않은 코드를 반복해서 공개한다면 그 회사는 오픈소스 세에서 신뢰를 잃게 되고, 나중에는 다른 코드를 오픈소스로 공개하여도 개발자는 관심을 두지 않을 것입니다.
