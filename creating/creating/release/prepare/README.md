---
description: 오픈소스 공개를 위해 준비해야 할 사항들을 설명합니다.
---

# 준비

SK텔레콤은 오픈소스를 통해 가치 창출을 기대하며 이를 적극 지원합니다. SK텔레콤의 소프트웨어를 오픈소스로 공개하기 위해 다음의 사항들을 준비합니다. 

## 프로젝트 이름 정하기

프로젝트의 이름은 시장에서 일관된 메시지를 보장하는 데 도움이 되기 때문에 특히 중요합니다. 프로젝트가 무엇인지 나타내는데 도움이 되는 이름을 사용하는 것이 좋습니다. 이와 함께 문제가 될 소지가 있는 이름을 피하기 위해 다음 페이지의 가이드를 따르세요. 

{% page-ref page="brand.md" %}

{% hint style="warning" %}
Repository 이름의 경우, 하이픈 \("-"\)으로 구분합니다. 

**DON'T** : successortoserverless  
**DO** : successor-to-serverless
{% endhint %}

## 라이선스 부여하기

소프트웨어를 오픈소스로 공개하기 위해서는 라이선스를 명시해야 합니다. 그래야 다른 사람들이 소프트웨어를 사용, 복사, 수정 및 배포할 수 있습니다. 또한, 라이선스는 법적인 문제로부터 당신을 보호합니다. 따라서, 오픈소스 프로젝트를 시작할때 적절한 오픈소스 라이선스를 선택하고 이를 프로젝트에 포함시켜야 합니다. 

SK텔레콤은 소프트웨어를 오픈소스로 공개 시 기본적으로 [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)를 적용합니다. Apache-2.0는 사용자에게 광범위한 자유를 제공하면서 명시적인 특허 허여 조항 등 법적인 관점에서도 가장 적절한 라이선스입니다. 

예외적으로 다음과 같은 경우는 Apache-2.0 외의 라이선스도 적용할 수 있습니다.  

* 커뮤니티에서 주로 사용하는 라이선스가 지정되어 있는 경우도 있습니다. 예를 들어,  Node.JS 프로젝트는 MIT 라이선스를 사용합니다. 이때는 해당 라이선스를 적용할 수 있습니다. 
* 어떤 프로젝트는 GPL 라이선스의 라이브러리와의 종속성이 있어서 GPL로 공개해야 하는 경우도 있습니다. 이것도 괜찮습니다. 

만약, 이외의 다른 라이선스를 선택해야 할 상황이라면 OSPO \(Open Source Program Office : ospo@sktelecom.com\)에 문의하시기 바랍니다.

{% hint style="warning" %}
오픈소스 공개 시 라이선스 선택에 대한 안내는 GitHub에서 제공하는 라이선스 선택 가이드를 참고할 수 있습니다. : [https://choosealicense.com](https://choosealicense.com)
{% endhint %}

## 공개할 소스 코드 준비하기

코드를 공개적으로 배포할 때에는 매우 주의해야 합니다. 코드 내 모든 주석이 공개하기에 적합한지, 보안 이슈는 없는지 확인합니다. 이 부분은 OSPO팀의 검토에만 의존하지 마세요. OSPO팀은 라이선스와 법적인 문제를 위주로 검토하지만, 모든 문제를 확인하지는 못합니다.

### 1\) 출처 확인

오픈소스 프로젝트에서 발생할 수 있는 최악의 상황 중 하나는 법적으로 문제가 있는 코드가 프로젝트에 포함되는 것입니다. 회사가 배포할 권리가 없는 코드이거나, 다른 회사의 특허와 같은 IP를 침해하는 코드가 법적인 문제를 유발시킬 수 있습니다. 따라서, 공개할 코드를 준비하면서 모든 코드의 출처를 확인하고 문제 소지가 있는 코드는 삭제해야 합니다.

\(haksung : Protex 사용하여 출처 확인하는 과정 추가 안내 필요\)

### 2\) 3rd party 코드는 별도 디렉토리에 모으세요. 

프로젝트에 3rd party 코드를 포함해야 하는 경우라면, 즉 SK텔레콤이 저작권을 갖고 있지 않은 코드를 프로젝트에 포함해야 한다면 SK텔레콤 코드와 다른 디렉토리\(예: third\_party\)에 위치시킵니다. 이는 라이선스 관점에서 프로젝트의 투명성을 증대시키며, 향후 사용자도 3rd party 코드를 쉽게 찾게 찾게 되어 정확한 라이선스 요구사항을 준수할 수 있게 합니다. 

3rd party 라이브러리에서 복사하거나 파생된 모든 파일은 역시 third\_party 디렉토리에 저장되어야 합니다. 3rd party 디렉토리에 있는 모든 디렉토리는 각각 LICENSE 파일 \(저작권 정보와 라이선스 전문을 포함하는 텍스트 파일\)을 포함해야 합니다. 

예를 들어, Repository에서 third\_party 디렉토리의 구조는 다음과 같습니다. 

```text
[Root Directory]
|-- Google source code
|-- ....
`-- third_party
    `-- [external library A]
    |   |-- `LICENSE`
    |   `-- ...
    `-- [external library B]
        |-- `LICENSE`
        `-- ...
```

프로젝트가 Dependency를 다운로드 및 사용하기 위한 Package Manager를 사용한다면, Dependency 분석\(haksung : dependency 분석 방법 추가 필요\)등의 방법을 수행하여 프로젝트의 Repository에 3rd party 코드가 포함되지 않게 합니다. 

### 3\) 주석을 정리하세요. 

* \(굳이 외부에 공개할 필요가 없는\) SK텔레콤 구성원의 이름과 이메일 주소를 삭제하세요. 
* 내부 정보를 삭제하세요. \(내부 코드 파일 이름 / 경로, 내부 호스트 / IP정보 등\)

참고로, 아래의 명령어를 사용하면, 불필요한 주석을 쉽게 찾을 수 있습니다.

* 회사 웹사이트, 이메일, IP 주소 검색

```text
$ egrep -r '\.sktelecom\.com|@sk\.com|@sktelecom\.com|([0-9]+\.){3}[0-9]+' <path-to-source-directory>
```

* Java/C/C++/Go/Objective-C/Objective-C++/Swift/Kotlin 주석 검색

```text
$ find <path-to-source-dir> -type f | egrep '\.(c|cc|h|cpp|go|java|kt|m|mm|swift)' | while read f; do echo "------------ $f ------------------"; sed -n -e '/\/\*.*\*\// {p; b}' -e '/\/\*/,/\*\//p' -e '/\/\//p' "$f"; done
```

* Python/Bash 주석 검색

```text
$ find <path-to-source-dir> -type f | egrep '\.(py|sh)' | while read f; do echo "------------ $f ------------------"; grep -o "#.*" "$f"; done
```

### 4\) README 파일을 포함하세요. 

우리가 공개한 오픈소스를 많은 사용자들이 사용하기를 원하나요? 그렇다면 사람들이 쉽게 시작할 수 있도록 README 파일을 제공하세요. README에 대한 자세한 내용은 다음 페이지를 참고하세요. 

{% page-ref page="readme.md" %}

### 5\) 라이선스 파일을 포함하세요

라이선스 사본을 담고 있는 LICENSE라는 이름의 텍스트 파일을 최상위 디렉토리에 포함합니다. 

* Apache License의 경우, [공식 라이선스 사본 파일](http://www.apache.org/licenses/LICENSE-2.0.txt)을 그대로 복사해서 사용하면 됩니다.
* 다른 라이선스를 적용하기로 한 경우, 라이선스 사본은 [SPDX License List](https://spdx.org/licenses/)에서 받을 수 있습니다. 

### 6\) 저작권 및 라이선스를 표하세요

소스 코드를 포함하는 모든 파일은 저작권 및 라이선스 표기를 포함해야 합니다. 이는 몇몇 파일만 복사해서 사용하려는 사용자들도 라이선스 의무를 준수하는데 도움이 됩니다. 자세한 내용은 다음 페이지를 참고하세요. 

{% page-ref page="mark.md" %}

### 7\) CONTRIBUTING 파일을 포함하세요

기여자들이 참고할 수 있는 "How to Contribute"에 대한 내용을 제공하는 파일입니다. CONTRIBUTING 파일이 충실하지 않다면 프로젝트로의 기여에 관심이 있던 사용자들도 열정을 잃게 됩니다. CONTRIBUTING 파일에 대한 자세한 내용은 다음 페이지를 참고하세요. 

{% page-ref page="contributing.md" %}

### 8\) CLA 파일을 포함하세요

일반적인 오픈소스 라이선스는 기여자로부터의 라이선싱도 명시하고 있기 때문에 추가적인 Contributor Agreement가 필요하지 않습니다. 필요에 따라 코드의 법적 문제를 방지하기 위해 기여자에게 CLA \(Contributor License Agreement\)나 DCO\(Developer Certificate of Origin\)를 요구하는 것도 고려할 수 있습니다. CLA와 DCO에 대한 세부 내용은 다음 페이지를 참고하세요. 

\(haksung : 어떤 CLA를 SK텔레콤 기본으로 할지에 대한 법무 검토 필요\)

{% page-ref page="cla.md" %}

### 9\) Code of Conduct 파일을 포함하세요 \(선택 사항\)

\(haksung : SK텔레콤의 Code of Conduct 작성 필요\)

{% page-ref page="conduct.md" %}

{% hint style="warning" %}
여기까지 준비가 됐으면 TDE &gt; OSPO &gt; Jira Ticke을 생성하여 OSPO 승인을 요청할 수 있습니다. 

\(haksung : 승인 요청 방법 구체화 필요\)
{% endhint %}

## 추가 사항

\(haksung : 아래 사항들을 가이드에 포함할지는 추가 검토 필요\)

### 리더쉽과 거버넌스 체계 수립

거버넌스는 프로젝트가 전략, 릴리스, 방향 및 개발 우선순위에 관한 결정을 내리는 프로세스입니다. 

모든 참여자가 프로젝트의 변경 사항을 인식할 수 있도록 의사 결정은 공개적이고 투명해야 합니다. 거버넌스 기구에 참여하기 위해 충족해야 할 기준을 결정하고, 기능 및 버그 추적 방법, 코드 제출 방법 및 릴리스 프로세스 관리에 대한 결정 방법을 수립합니다. 

또한, 프로젝트를 시작하기 전에 리더쉽 역할을 정하는 것도 중요합니다. 여러 기업 참가자와 함께 프로젝트를 시작하는 경우 프로젝트에는 관리 위원회 \(Governing Board\)와 같은 공식적인 거버넌스 조직이 필요할 수 있습니다.

이에 대한 자세한 내용은 다음 페이지를 참고하세요. 

{% page-ref page="../../governance.md" %}

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

### 마케팅

런칭이 단계의 마지막이 아닙니다. 프로젝트를 계속 진행하기 위해서는 마케팅 단계가 필수적입니다. 

마케팅에는 프로젝트 홍보, 성공적인 운영 전략 수립, 현실적인 예산 및 프로젝트 브랜딩 제공, 소셜 미디어 계정 활성화 등 장기적인 성공을 위한 활동 등이 포함됩니다. 일반적인 마케팅 검토 절차는 다음과 같습니다. 

1. 프로젝트 로고, Color Scheme, 웹사이트 등을 디자인하세요. 
2. 소셜 미디어 계정을 등록하세요. \(Twitter, Facebook, LinkedIn 등\)
3. Domain Name을 등록하세요.

{% hint style="success" %}
이 페이지는 다음 문서를 참고하였습니다. : [https://opensource.google/docs/releasing/](https://opensource.google/docs/releasing/)
{% endhint %}

