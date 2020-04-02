# 저작권 및 라이선스 표기



{% hint style="warning" %}
* [https://opensource.google/docs/releasing/licenses/](https://opensource.google/docs/releasing/licenses/)
* [https://opensource.google/docs/releasing/preparing/](https://opensource.google/docs/releasing/preparing/)
* [https://matija.suklje.name/how-and-why-to-properly-write-copyright-statements-in-your-code](https://matija.suklje.name/how-and-why-to-properly-write-copyright-statements-in-your-code)
{% endhint %}

저작권은 \([베른 협약](https://en.wikipedia.org/wiki/Berne_Convention) 이후\) 저작자가 저작물 만들 때 자동으로 생성됩니다. 모든 저작물은 저작권에 의해  보호되며, 저작권 보유자에게 저작물에 대한 독점적인 권한이 부여됩니다. 따라서 당신의 저작물\(소스 코드, 텍스트, 이미지, 기타 미디어 등\)을 다른 사용자가 사용할 수 있게 하려면 그들에게 라이선스를 부여해야 합니다. 라이선스의 사전적 정의는 "특정 권리를 실행하기 위해 자격이 있는 기관으로부터 받은 허가"이며, 이러한 허가 없이 특정 권리를 실행하는 것은 저작권 침해와 같은 불법 행위가 됩니다. 

저작권 표시가 법에 따라 요구되는 것은 아니지만, \(1\) 대부분의 오픈소스 라이선스가 저작권 표시를 요구하고, \(2\) 사용자가 법적 또는 기술적인 이유로 저작권자에게 연락하기를 원할 수 있다는 점을 고려하여 소스 코드 파일에 저작권 표시를 포함하는 것은 의미가 있습니다. 

SK텔레콤에서 작성하여 오픈소스로 공개하는 모든 소스 코드 파일은 다음과 같은 방법으로 저작권 표시 및 라이선스를 고지하세요. 

## 저작권 표시

소스 코드 상단 헤더 부분에 다음 정보를 포함하는 저작권 표시를 추가하세요. 

* © 기호
* 최초 작성 연도
* 저작권 보유자 이름
  * SK텔레콤 구성원이 저자인 저작물의 저작권은 SK텔레콤이 보유합니다. 따라서, 회사 이름을 작성합니다. \(SK TELECOM CO., LTD.\)
* 연락처 \(Optional\)
  * 사용자가 저자에게 기술적, 법률적 문의를 위해 연락을 취하고 싶을 수 있습니다. 이를 대응하기 위한 저자의 이메일 정보를 제공할 수 있습니다. 이는 필수는 아닙니다. 
  * 또는, 사용자가 정보를 얻을 수 있는 프로젝트의 웹사이트 URL 등 연락처 정보를 작성합니다.

저작권 표시는 [REUSE.software](https://reuse.software/) 프로젝트에서 권장하는 방법인 SPDX Tag \("SPDX-FileCopyrightText"\)를 사용하여 표시합니다. 그 예는 아래와 같습니다. 

```text
SPDX-FileCopyrightText: © 2020 SK TELECOM CO., LTD. <{$project-website-url}>
```

## 라이선스 고지

각 소스 코드 파일마다 라이선스가 무엇인지 알리는 것도 매우 중요합니다. 라이선스는 혼란을 줄이기 위해 Linux Foudnation의 [SPDX](https://spdx.org/) 프로젝트에서 제공하는 [SPDX ID를](https://spdx.org/ids) 사용하여 표시합니다. SPDX ID를 사용하는 방법은 간단합니다. 

먼저 적용하고자 하는 오픈소스 라이선스의 SPDX Identifier가 무엇인지 [SPDX License List](https://spdx.org/licenses/) 페이지에서 확인합니다. 예를 들어, Apache License version 2의 SPDX Identifier는 Apache-2.0입니다.

![](https://t1.daumcdn.net/thumb/R1280x0/?fname=http%3A%2F%2Ft1.daumcdn.net%2Fbrunch%2Fservice%2Fuser%2F9399%2Fimage%2F52k_mIfC4DbQz9aZf9Eteb3PH6A.png)

그리고 소스 코드 파일 상단에 SPDX-License-Identifier라는 tag를 이용하여 라이선스 Identifier를 표시합니다. 그 예는 아래와 같습니다. 

```text
SPDX-License-Identifier: Apache-2.0
```







