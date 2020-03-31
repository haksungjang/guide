---
description: Releasing new open source projects
---

# 오픈소스 공개

{% hint style="warning" %}
[https://opensource.google/docs/releasing/](https://opensource.google/docs/releasing/)
{% endhint %}

여기서는 새로운 오픈소스를 공개하는 절차에 대해 설명합니다. \(여기서 '공개'라는 말은 GitHub과 같은 Repository에 소프트웨어를 등록하여 누구나 접근할 수 있게 하는 것을 의미합니다.\)\

새로운 오픈소스를 공개하는 개략적인 절차는 다음과 같습니다. 

## Quick Overview

### 1. 준비하기

1. [프로젝트 이름을 정하세요](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#undefined). 
2. [회사 정보가 있는 코드와 주석을 지우세요.](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#3)
3. [README 파일](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#4-readme)을 포함하세요.
4. [오픈소스 라이선스](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#undefined-1)를 선택하고, [소스 파일 헤더](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#6)에 포함하세요. 
5. [CONTRIBUTING](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#7-contributing) 파일을 포함하세요.
6. 회사 구성원이 작성하지 않은 코드는 [third\_party 디렉토리](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#2-3rd-party)에 있도록 하세요. 

이에 대한 자세한 사항은 다음 페이자를 참고하세요.

{% page-ref page="prepare/" %}

{% hint style="warning" %}
[https://github.com/google/new-project](https://github.com/google/new-project) 에서 오픈소스 공개를 위한 템플릿이 제공됩니다.    
\(haksung : SK텔레콤 내용으로 변경 필요\)
{% endhint %}

### 2. 검토 요청하기

1. 내부 Git Repository에 코드를 등록하세요. \(haksung : 사내 Git Repository에 대한 정보 추가 필요\)
2. 오픈소스 검사 도구 \(haksung : Black Duck 사용 방법에 대한 추가 안내 필요\)로 Repository를 검사하고 발견된 이슈를 해결합니다. 
3. 사내 오픈소스팀에 검토를 요청하세요. \(haksung : 검토 요청 방법에 대해 추가 필요\)

### 3. 승인 받기

\(haksung : SKT 상황에 맞게 보완\)

{% page-ref page="approval.md" %}

### 4. 공개 하기

{% hint style="warning" %}
중요 : 다음 사항은 승인을 받은 후 진행하세요.
{% endhint %}

1. 외부 Repository를 새성합니다. 
2. Repository에 코드를 Push합니다. 
3. \(작성 중\)

{% page-ref page="releasing.md" %}



## Patching

만약, 다음 경우에 해당한다면 기여하기 절차를 따릅니다. 

1. \(기여의 규모나 복잡성에 관계 없이\) 기존 오픈소스 프로젝트에 기여하는 경우
2. 100 라인 이하의 코드 조각을 공개하는 경우
3. StckOverflow에 코드를 게시하는 경우
4. 오픈소스 프로젝트의 관리자로 역할을 수행하는 경우

{% page-ref page="../../../contribute/main/" %}

## Need help?

도움이 필요하세요? opensource@sk.com으로 연락주세요. \(haksung : 공식적인 창구 확인 필요. 이메일로 할지, TDE를 통할지?\)

