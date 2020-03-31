# 공개

{% hint style="warning" %}
[https://opensource.google/docs/releasing/publishing/](https://opensource.google/docs/releasing/publishing/)
{% endhint %}

공개\(Releasing\)는 ['오픈소스 공개](https://opensource-skt.gitbook.io/guide/creating/creating/release)'의 한 단계로써 승인을 받은 후 진행하며 다음 단계를 따릅니다. 

## 암호화 컴플라이언스 \(Cryptography compliance\)

오픈소스로 공개하는 프로젝트에 암화화 \(cryptographic\) 관련 소프트웨어가 포함된다면 수출 규제 \(Export Control\) 준수팀에 문의할 필요가 있습니다. 단, 프로젝트가 인증\(authentication\)이나 디지털 서명\(digital signature\) 관련 기능만 제공한다면 문의하지 않아도 됩니다. 

그러나, 다음과 같은 데이터 암호화\(data encryption\)를 수행하거나 사용한다면 수출 규제 준수팀에 이를 알리고 적절한 조치를 취하여야 합니다. 

* 암호화 라이브러리 \(crypto library\) 제공
* https, OpenSSL, OpenVPN 이나 기타 암호화 프로토콜 \(encryption protocal\)을 이용하여 데이터 암호화 수행

수출 규제 준수팀에 이를 알릴 때에는 다음 정보를 함께 제공합니다. 

* 프로젝트 관리자 이름
* 프로젝트 이름
* 소스 코드를 다운로드 받을 수 있는 URL

\(haksung : 수출 규제 준수 관련 담당부서가 회사 내에 있는지, 있다면 어디인지 확인 후 연락처 업데이트 필요\)

## 커뮤니케이션 채널

커뮤니티에서 원활한 커뮤니케이션이 가능하도록 채널을 제공하는 것이 중요합니다. 또한 코드 체크인, 오류 로그 등 기타 작업에 대한 알림을 주는 등 전체 개발 Work Flow에 통합할 수 있는 도구가 필요합니다. 이는 프로젝트를 실시간으로 진행하는 중요한 수단이 됩니다. 

* 우수한 도구 중 하나는 [Slack](https://slack.com/)입니다. Slack은 사용자가 메시지와 파일을 공유하고, Work Flow 구성, 정보 검색 등의 작업을 수행할 수 있게 하는 온라인 프로젝트 관리 및 통신 플랫폼입니다. 그러나 Slack은 상용 도구이며 유지 관리 비용이 발생합니다. 
* 오픈소스로 공개된 도구들로는 IRC, [Gitter.im](https://gitter.im/), [Rocket.Chat ](https://rocket.chat/)등이 있습니다. Rocket.Chat은 오픈소스이며 Slack과 유사한 기능을 제공합니다. 

단, Slack과 같은 타사 서비스에서는 회사의 기밀 정보를 논의해서는 안됩니다. 이러한 커뮤니케이션 채널은 공개 토론으로만 사용해야하며 회사 내부 조직의 논의 도구로는 사용할 수 없습니다. 

## Repository 생성과 코드 공개

모든 준비와 검토 및 승인 단계를 마친 후에는 repository를 생성합니다. \(haksung : sk github repository를 사용할 수 있도록 추가 안내 필요\) 

그리고, 오픈소스 프로젝트를 공개합니다. 소스 코드를 repository에 릴리즈하세요. 

이제, 오픈소스 개발 모델을 따라 프로젝트를 운영합니다. 

## 마케팅

프로젝트를 계속 진행하기 위해서는 마케팅 필수적입니다. 

마케팅에는 프로젝트 홍보, 성공적인 운영 전략 수립, 현실적인 예산 및 프로젝트 브랜딩 제공, 소셜 미디어 계정 활성화 등 장기적인 성공을 위한 활동 등이 포함됩니다. 여기에서는 프로젝트를 공개하고 이를 알리기 위한 몇가지 방법을 안내합니다. 

1. 프로젝트와 관련이 있는 커뮤니티의 메일링 리스트나 포럼에 프로젝트가 공개되었음을 알립니다. 
2. SK텔레콤 기술 블로그에 프로젝트에 대해 소개합니다. 
3. SK텔레콤 소셜 미디어\(Twitter, Facebook, LinkedIn 등\)를 통해 홍보합니다. 또한 프로젝트 자체의 소셜 미디어 계정을 생성하여 지속적으로 활동합니다. 
4. 프로젝트와 관련이 있는 오픈소스 컨퍼런스에서 주제 발표를 합니다. 

