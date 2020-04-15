# 오픈소스 사용하기 \(작성 중\)

오픈소스를 사용하지 않고 제품이나 서비스를 개발하는 것은 불가능하다고 할 수 있을 만큼 소프트웨어 개발에 오픈소스는 핵심 요소가 되었습니다. 오픈소스의 사용으로 소프트웨어 개발 시간을 단축하면서도 서비스 안정성 및 보안 강화를 기대할 수 있습니다. 하지만, 오픈소스를 사용할 때는 라이선스가 무엇인지 확인하고, 라이선스가 요구하는 의무사항을 준수해야 합니다. 

이 가이드는 오픈소스를 사용하면서 주의해야 할 사항들을 안내합니다.  

## 오픈소스 사용 책임 

소프트웨어를 개발하면서 문제 해결을 위해 널리 채택되고 있는 오픈소스가 있다면 이를 채택하여 적용하는 것이 자체 구현하는 것보다 개발 속도와 안정성 측면에서 훨씬 유리합니다. 어떤 오픈소스가 기능/성능/보안/안정성 측면에서 우수한지에 대해 판단하는 건 오픈소스를 사용하는 개발자의 책임입니다. \(T hub의 기술 커뮤니티 혹은 협업 기능을 통해 각 기술 분야의 마스터에게 문의할 수 있습니다.\) 

SK텔레콤의 OSPO \(Open Source Program Office\)는 라이선스 관련하여 도움을 제공합니다. 오픈소스를 사용하면서 라이선스 측면에서 문의가 있다면 TDE &gt; OSPO에 Ticket을 생성하여 문의하세요. 

## 저작권 

당신이 독창적인 저작물 \(예: 글, 그림, 코드 등\)을 만들면, 그 저작물은 자동으로 저작권의 보호를 받습니다. 즉, 그 저작물은 다른 사람이 임의로 사용, 복사, 수정 또는 배포할 수 없습니다. 

## 라이선스

라이선스는 자신의 저작물을 다른 사람이 사용, 복사, 수정, 배포 등을 할 수 있도록 허가하는 것을 말합니다. 

## 오픈소스

오픈소스는 많은 사람들이 자유롭게 사용, 수정하고 배포도 할 수 있게 하는 것인데요, 이를 위해서는 이러한 권한을 명시적으로 나타내는 오픈소 라이선스가 필요합니다. 따라서, 오픈소스 라이선스가 적용되지 않은 소프트웨어는 오픈소스가 아니며, 저작권자를 제외한 누구도 그 소프트웨어를 사용, 복제, 수정 및 배포할 수 없습니다. 

{% hint style="warning" %}
예를 들어, GitHub에 프로젝트를 공개하였다고 해서 오픈소스인 것은 아닙니다. GitHub의 Public 프로젝트는 [GitHub’s Terms of Service](https://help.github.com/en/github/site-policy/github-terms-of-service#3-ownership-of-content-right-to-post-and-license-grants)가 적용되어서 다른 사람들이 당신의 프로젝트를 보거나 Fork 할 수는 있지만 다른 권한은 부여하지 않습니다. 당신의 프로젝트가 많은 사람들이 자유롭게 사용, 수정, 배포하고 또다시 기여하기를 바란다면 오픈소스 라이선스를 적용해야 합니다. 
{% endhint %}

## 오픈소스 라이선스 

다양한 오픈소스 라이선스가 있지만, 오픈소스 라이선스 들의 주요 목적은 동일합니다. 바로 다른 사람들이 코드를 사용할 수 있도록 하는 것입니다. 단, 코드를 사용할 때 준수해야 할 의무 사항은 오픈소스 라이선스 별로 차이가 있음에 주의해야 합니다.

{% hint style="warning" %}
**라이선스가 없는 코드라면?**

만약 당신이 찾은 코드에 라이선스가 명시되어 있지 않다면, 그 코드를 사용할 수 있는 권리는 여전히 저작권자에게만 있다는 것입니다. 따라서, 당신은 그 코드를 사용할 권리가 없습니다. 그 코드를 회사의 제품 혹은 서비스에 포함시킬 수 없습니다. 꼭 필요한 코드라면 코드의 저작자에게 연락하여 다음과 같이 요청하세요. 

_We’d love to use this code in a project of ours and wanted to make sure that you are OK with it. Would you be willing to add an OSI-approved license like the MIT or the Apache License to the project so that we know this is really open source?_

대부분의 저작자들은 이에 대해 긍정적으로 대응할 것입니다. 
{% endhint %}

## 라이선스 확인

인터넷에서 사용할 코드를 찾으면 먼저 라이선스를 확인하세요. 확인 방법은 다음 페이지를 참고하세요. \(haksung : 추가 작성 필요\)

## 오픈소스 라이선스 유형

일반적인 오픈소스 라이선스의 유형은 다음과 같습니다.

### Permissive  라이선스

Permissive  라이선스는 코드 사용을 허가하며 최소한의 의무\(고지 의무\)를 부과하여 상대적으로 준수하기가 쉽습니다. 다음과 같은 오픈소스 라이선스를 Permissive 라이선스로 분류할 수 있습니다. 

* MIT
* BSD
* Apache-2.0
* ISC
* zLib
* JSON
* CC-BY \(Creative Commons Attribution\)
* SIL Open Font

 Permissive 라이선스가 부여된 코드는 비교적 자유롭게 제품 및 서비스에 사용할 수 있습니다. 세부 절차는 다음 가이드를 참고하세요. \(haksung : 회사 정책에 맞게 가이드 추가 작성 필요 / 참고 : [https://verizonmedia.github.io/oss-guide/docs/launching/mobile.html](https://verizonmedia.github.io/oss-guide/docs/launching/mobile.html)\)

1. 모바일 애플리케이션에 오픈소스 사용 시 의무 사항 준수 방안 
2. 임베디드 소프트웨어를 포함하는 제품에 오픈소스 사용 시 의무 사항 준수 방안
3. 서버 프로그램에 오픈소스 사용 시 의무 사항 준수 방안

### Copyleft 라이선스

\(haksung : 추가 작성 필요\)



{% hint style="success" %}
이 페이지는 다음 문서를 참고하였습니다. 

* [https://opensource.guide/legal/](https://opensource.guide/legal/)
* [https://verizonmedia.github.io/oss-guide/docs/using/using.html](https://verizonmedia.github.io/oss-guide/docs/using/using.html)
{% endhint %}







