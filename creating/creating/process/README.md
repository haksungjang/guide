---
description: Releasing new open source projects
---

# 절차와 방법

여기서는 새로운 오픈소스를 공개하는 절차에 대해 설명합니다. \( '공개'는 GitHub과 같은 Repository에 소프트웨어를 등록하여 누구나 접근할 수 있게 하는 것을 의미합니다.\)

새로운 오픈소스를 공개하기 위한 주요 3단계는 다음과 같습니다. 

## 1단계. 준비

1. [프로젝트 이름을 정하세요](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#undefined). 
2. [라이선스를 부여하세요.](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#undefined-1)
3. [공개할 소스 코드를 준비하세요.](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#undefined-2)
   1. 출처확인
   2. 3rd party 코드 확인
   3. [회사 정보가 있는 코드와 주석 제거](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#3)
   4. [README 파일](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#4-readme) 포함
   5. LICENSE 파일 포함
   6. [소스 파일 헤더](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#6)에 저작권과 라이선스 표시
   7. [CONTRIBUTING](https://opensource-skt.gitbook.io/guide/creating/creating/release/prepare#7-contributing) 파일 포함
   8. CLA 파일 포
   9.  Code of Conduct 파일 포
4. [보안 취약점](https://opensource-skt.gitbook.io/guide/creating/creating/process/prepare#undefined-3)을 점검하세요.
5. [암호화 컴플라이언스](https://opensource-skt.gitbook.io/guide/creating/creating/process/prepare#cryptography-compliance)를 확인하세요.
6. [커뮤니케이션 채널](https://opensource-skt.gitbook.io/guide/creating/creating/process/prepare#undefined-4)을 준비하세요.
7. [리더쉽과 거버넌스 체계](https://opensource-skt.gitbook.io/guide/creating/creating/process/prepare#undefined-4)를 수립하세요.
8. [인프라](https://opensource-skt.gitbook.io/guide/creating/creating/process/prepare#undefined-6)를 구축하세요. 
9. [웹사이트](https://opensource-skt.gitbook.io/guide/creating/creating/process/prepare#undefined-7)를 구축하세요. 

이에 대한 자세한 사항은 다음 페이지를 참고하세요.

{% page-ref page="prepare/" %}

{% hint style="warning" %}
[https://github.com/google/new-project](https://github.com/google/new-project) 에서 오픈소스 공개를 위한 템플릿이 제공됩니다.    
\(haksung : SK텔레콤 내용으로 변경 필요\)
{% endhint %}

## 2단계. 승인

1단계 준비가 완료되면 TDE &gt; OSPO &gt; Jira Ticket을 생성하여 OSPO 승인을 요청합니다. 

{% page-ref page="approval.md" %}

## 3단계. 공개

{% hint style="warning" %}
이 단계는 반드시 승인을 받은 후 진행하세요.
{% endhint %}

{% page-ref page="release.md" %}

## Need help?

도움이 필요하세요? TDE &gt; OSPO에 Ticket을 생성하여 문의 및 요청하세요. 

{% hint style="success" %}
이 페이지는 다음 문서를 참고하였습니. : [https://opensource.google/docs/releasing/](https://opensource.google/docs/releasing/)
{% endhint %}

