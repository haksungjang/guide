# 공개할 코드 준비

코드를 공개적으로 배포할 때에는 매우 주의해야 합니다. 코드 내 모든 주석이 공개하기에 적합한지, 보안 이슈는 없는지 확인합니다. 이 부분은 OSPO팀의 검토에만 의존하지 마세요. OSPO팀은 라이선스와 법적인 문제를 위주로 검토하지만, 모든 문제를 확인하지는 못합니다.

코드를 공개적으로 배포할 때에는 매우 주의해야 합니다. 코드 내 모든 주석이 공개하기에 적합한지, 보안 이슈는 없는지 확인합니다. 이 부분은 OSPO팀의 검토에만 의존하지 마세요. OSPO팀은 라이선스와 법적인 문제를 위주로 검토하지만, 모든 문제를 확인하지는 못합니다.

## 1. 출처 확인 <a id="id-&#xACF5;&#xAC1C;&#xD560;&#xCF54;&#xB4DC;&#xC900;&#xBE44;-1.&#xCD9C;&#xCC98;&#xD655;&#xC778;"></a>

‌오픈소스 프로젝트에서 발생할 수 있는 최악의 상황 중 하나는 법적으로 문제가 있는 코드가 프로젝트에 포함되는 것입니다. 회사가 배포할 권리가 없는 코드이거나, 다른 회사의 특허와 같은 IP를 침해하는 코드가 법적인 문제를 유발시킬 수 있습니다. 따라서, 공개할 코드를 준비하면서 모든 코드의 출처를 확인하고 문제 소지가 있는 코드는 삭제해야 합니다.‌ 

## 2. 코드 품질 검토 <a id="id-&#xACF5;&#xAC1C;&#xD560;&#xCF54;&#xB4DC;&#xC900;&#xBE44;-2.&#xCF54;&#xB4DC;&#xD488;&#xC9C8;&#xAC80;&#xD1A0;"></a>

‌코드의 가독성과 성숙도는 오픈소스로 공개하기 위한 준비가 되었는지에 대한 척도가 됩니다. 성숙하지 않은 코드는 커뮤니티의 신뢰를 잃게 합니다.

그렇다고 코드가 완벽해야 한다는 건 아닙니다. 코드를 완벽하게 준비하려고 한다면 아마 시작할 수도 없을 것입니다. 주어진 환경에서 최선의 수준으로 준비하여 공개하세요. 커뮤니티가 활성화되면 외부 기여자들이 코드를 개선하는 데 참여할 것입니다. 

## 3. 3rd party 코드 확인 <a id="id-&#xACF5;&#xAC1C;&#xD560;&#xCF54;&#xB4DC;&#xC900;&#xBE44;-3.3rdparty&#xCF54;&#xB4DC;&#xD655;&#xC778;"></a>

‌프로젝트에 3rd party 코드를 포함해야 하는 경우라면, 즉, SK텔레콤이 저작권을 갖고 있지 않은 코드를 프로젝트에 포함해야 한다면 먼저 SK텔레콤이 배포할 수 있는 권한이 있는지 확인하세요. 이미 오픈소스 라이선스가 적용된 코드라면 라이선스 의무를 준수하는 조건으로 배포할 수 있습니다. 배포할 수 있는 권한 확인에 대한 도움이 필요하다면 T-DE &gt; OSP \(_https://tde.sktelecom.com/pms/projects/OSP/issues_\)에 새 이슈를 생성하여 문의하세요.

SK텔레콤이 배포할 수 있는 3rd party 코드인 경우, 기존 코드와는 다른 디렉토리\(예: third\_party\)에 위치시킵니다. 이는 라이선스 관점에서 프로젝트의 투명성을 증대시키며, 향후 사용자도 3rd party 코드를 쉽게 찾게 찾게 되어 정확한 라이선스 요구사항을 준수할 수 있게 합니다.

3rd party 디렉토리에 있는 모든 디렉토리는 각각 LICENSE 파일 \(저작권 정보와 라이선스 전문을 포함하는 텍스트 파일\)을 포함해야 합니다. 예를 들어, Repository에서 third\_party 디렉토리의 구조는 다음과 같습니다.

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

## 4. 주석 정리 <a id="id-&#xACF5;&#xAC1C;&#xD560;&#xCF54;&#xB4DC;&#xC900;&#xBE44;-4.&#xC8FC;&#xC11D;&#xC815;&#xB9AC;"></a>

공개하려는 코드에 회사의 영업 비밀이나 문제를 일으킬만한 불필요한 주석이 포함되지 않도록 확인하세요.‌

* \(굳이 외부에 공개할 필요가 없는\) SK텔레콤 구성원의 이름과 이메일 주소를 삭제하세요.
* 내부 정보를 삭제하세요. \(내부 코드 파일 이름 / 경로, 내부 호스트 / IP정보 등\)

참고로, 아래의 명령어를 사용하면, 불필요한 주석을 쉽게 찾을 수 있습니다.

```text
### 회사 웹사이트, 이메일, IP 주소 검색
$ egrep -r '\.sktelecom\.com|@sk\.com|@sktelecom\.com|([0-9]+\.){3}[0-9]+' <path-to-source-directory>
 
### Java/C/C++/Go/Objective-C/Objective-C++/Swift/Kotlin 주석 검색
$ find <path-to-source-dir> -type f | egrep '\.(c|cc|h|cpp|go|java|kt|m|mm|swift)' | \
  while read f; do echo "------------ $f ------------------"; sed -n -e '/\/\*.*\*\// {p; b}' \
  -e '/\/\*/,/\*\//p' -e '/\/\//p' "$f"; done
 
### Python/Bash 주석 검색
$ find <path-to-source-dir> -type f | egrep '\.(py|sh)' | while read f; \
  do echo "------------ $f ------------------"; grep -o "#.*" "$f"; done
```

## **5. README 파일을 작성하세요.** 

우리가 공개한 오픈소스를 많은 사용자들이 사용하기를 원하나요? 그렇다면 사람들이 쉽게 시작할 수 있도록 README 파일을 제공하세요. README 파일은 새로운 사람들에게 프로젝트에 대해 설명하는 가장 중요한 문서입니다.

README에서는 다음 질문에 답할 수 있는 내용을 포함해야 합니다.‌

* 이 프로젝트는 무엇을 하는 프로젝트 인가요?
* 왜 이 프로젝트가 유용한가요?
* 어떻게 시작하면 되나요?
* 도움이 필요하면 어디서 도움을 받을 수 있나요?

프로젝트 사용자의 배경지식은 매우 다양합니다. 프로젝트를 막 시작하여 경험이 없는 사람도 쉽게 이해할 수 있도록 자세하게 문서를 제공하는 것이 좋습니다. 문서가 충실하게 제공될 수록 더 많은 사용자와 기여자를 확보할 수 있음을 기억하세요.

{% hint style="warning" %}
* README 템플릿 참고 : [README Template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* README 작성 가이드 참고 : [Make a README](https://www.makeareadme.com/)
{% endhint %}

## 6. 라이선스 파일을 포함하세요.

라이선스 사본을 담고 있는 LICENSE라는 이름의 텍스트 파일을 최상위 디렉토리에 포함합니다. 

* Apache License의 경우, [공식 라이선스 사본 파일](http://www.apache.org/licenses/LICENSE-2.0.txt)을 그대로 복사해서 사용하면 됩니다.
* 다른 라이선스를 적용하기로 한 경우, 라이선스 사본은 [SPDX License List](https://spdx.org/licenses/)에서 받을 수 있습니다. 

## 7. 저작권 및 라이선스를 표시하세요. 

소스 코드를 포함하는 모든 파일은 저작권 및 라이선스 표기를 포함해야 합니다. 이는 몇몇 파일만 복사해서 사용하려는 사용자들도 라이선스 의무를 준수하는데 도움이 됩니다. 자세한 내용은 다음 페이지를 참고하세요. 

{% page-ref page="copyright.md" %}

## 8. CONTRIBUTING 파일을 작성하세요. 

기여자들이 참고할 수 있는 "How to Contribute"에 대한 내용을 제공하는 파일입니다. CONTRIBUTING 파일이 충실하지 않다면 프로젝트로의 기여에 관심이 있던 사용자들도 열정을 잃게 됩니다. 

CONTRIBUTING 파일은 다음과 같은 사항을 포함합니다.

* 버그 리포트를 제출하는 방법 \(Issue 생성 / Pull Request 제출 방법\)
* 새로운 기능을 제하는 방법 
* 개발 환경을 설정하고 테스트를 실행하는 방법

또한, 다음과 같이 기여자들로부터 기여받기를 바라는 바에 대해 안내할 수 있습니다. 

* 원하는 기여 형태
* 프로젝트의 비전과 로드맵
* 기여자들이 프로젝트 관리자에게 연락을 취할 수 있는 방법

프로젝트의 초기 단계에서의 CONTRIBUTING 파일은 간단해도 됩니다. 단, 버그 리포트 및 이슈 제기 방법과 사전 테스트와 같이 기여를 하기 위한 필수 조건에 대해서는 꼭 설명해야 합니다.

그리고, 따뜻하고 친근한 분위기의 문서를 제공하세요. 이러한 문서가 잠재적인 기여자들에게 프로젝트에 참여하고 싶은 기분이 들게 합니다. 예를 들어, [Active Admin](https://github.com/activeadmin/activeadmin/)이라는 프로젝트의 [Contributing 가이드](https://github.com/activeadmin/activeadmin/blob/master/CONTRIBUTING.md)는 다음과 같이 시작합니다. 

> _"먼저 Active Admin에 기여하는 것을 고려해주셔서 감사합니다. Active Admin을 훌륭한 도구가 될 수 있는건 바로 당신 때문입니다!"_

{% hint style="warning" %}
* CONTRIBUTING 파일 템플릿 : [CONTRIBUTING-template.md](https://github.com/nayafia/contributing-template/blob/master/CONTRIBUTING-template.md)
* CONTRIBUTING 파일 \(예\) : 
  * Atom editor [contribution guidelines](https://github.com/atom/atom/blob/master/CONTRIBUTING.md).
  * Ruby on Rails [contribution guidelines](https://github.com/rails/rails/blob/master/CONTRIBUTING.md).
  * Open Government [contribution guidelines](https://github.com/opengovernment/opengovernment/blob/master/CONTRIBUTING.md).
{% endhint %}

CONTRIBUTING 파일도 README와 마찬가지로 프로젝트 Repository내 최상이 폴더에 위치시킵니다. 그리고, 사용자들이 접근하기 쉽도록 README 파일 내에 링크를 제공하세요. 

## 9. CLA 파일을 포함하세요 \(선택사항\)

일반적인 오픈소스 라이선스는 기여자로부터의 라이선싱도 명시하고 있기 때문에 추가적인 Contributor Agreement가 필요하지 않습니다. SK텔레콤이 공개하는 오픈소스 프로젝트는 일반적으로 CLA를 요구하지 않습니다. 다만, 필요에 따라 코드의 법적 문제를 방지하기 위해 기여자에게 CLA \(Contributor License Agreement\)나 DCO\(Developer Certificate of Origin\)를 요구하는 것도 고려할 수 있으며, 이 경우 OSPO에 문의하세요. 

CLA와 DCO에 대한 대략적인 사항은 아래 설명을 참고하세요. 

### CLA

어떤 프로젝트는 오픈소스 라이선스만으로는 명시적인 기여 조건이 불확실하다고 생각하기 때문에 모든 기여자에게 명시적인 CLA를 받기를 원합니다. 이정도의 요구사항을 충족할 수 있는 간결한 CLA\(Contributor License Agreement\)로 OpenJS의 Individual CLA를 참고할 수 있습니다. : [https://openjsf.org/wp-content/uploads/sites/84/2019/11/OpenJS-Foundation-Individual-CLA-2019-11-15.pdf](https://openjsf.org/wp-content/uploads/sites/84/2019/11/OpenJS-Foundation-Individual-CLA-2019-11-15.pdf)

### DCO

또 어떤 프로젝트는 개발자에게 그들이 만든 각 Commit에 대한 권한이 있음을 진술하기를 원합니다. [DCO](https://developercertificate.org/) \(Developer Certification Origin\)는 이런 요구사항을 충족하며, 많은 프로젝트에서 사용하고 있습니다. 

```text
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
1 Letterman Drive
Suite D4700
San Francisco, CA, 94129

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.


Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

* 한 예로, Node.js 커뮤니트는 CLA를 사용하다가 [DCO](https://github.com/nodejs/node/blob/master/CONTRIBUTING.md)로 [변경](https://nodejs.org/en/blog/uncategorized/notes-from-the-road/#easier-contribution)하였습니다. 
* GitHub Repository에서 DCO를 자동화하는 간단한 방법은 Bot을 이용하는겁니다.  : [Probot](https://github.com/probot/dco)

### Apache Individual CLA

MIT와 같은 오픈소스 라이선스는 명시적 특허 허여 조항을 포함하지 않습니다. 이런 오픈소스 프로젝트에서 만약 기여자로부터 명시적인 특허 허여를 받고 싶다면 [Apache Individual CLA](https://www.apache.org/licenses/icla.pdf) \(Contributor License Agreement\)를 사용할 수 있습니다. 이 CLA는 Apache License 2.0과 동일한 특허 허여 조항을 포함합니다. 

### Google CLA

Google의 CLA 전략을 참고하는 것도 도움이 됩니다. : [https://opensource.google/docs/releasing/contributions/](https://opensource.google/docs/releasing/contributions/)

이외에 다음 사항들도 고려할 수 있습니다. 

* 향후 라이선스 변경 필요성을 고려하여 기여자들에게 미리 이에 대한 동의를 받기 위한 내용을 CLA에 포함시킬 수 있습니다. 
* CLA 작성 시, [CLA assistant](https://github.com/cla-assistant/cla-assistant)를 이용하면 기여자의 혼란을 줄일 수 있습니다. 

## 10. Code of Conduct 파일을 포함하세요 \(선택 사항\)

\(작성 예정 : haksung@sk.com\) 

