# 오픈소스 라이선스

SK텔레콤의 구성원 외부로 배포하는 소프트웨어에 포함된 모든 오픈소스에 대해 라이선스 의무사항을 준수해야 합니다. 많은 오픈소스가 이미 광범위하게 사용되는 오픈소스 라이선스로 배포되기 때문에 라이선스 의무를 준수하는 과정은 일반적으로 간단합니다. 

이 문서는 오픈소스 라이선스가 무엇인지, 어떤 의무를 준수해야 하는지에 대한 자세한 정보를 제공합니다. 

SK텔레콤은 다음과 같이 오픈소스 라이선스를 분류하고 있습니다.

## Copyleft 라이선스 유형

Copyleft 라이선스 유형은 오픈소스 라이선스 중에 요구하는 의무사항이 가장 많은 라이선스 유형이기 때문에 이 유형의 라이선스로 배포되는 오픈소스는 사용 시 주의가 필요합니다. 

대표적인 의무 사항은 이 라이선스로 배포되는 오픈소스를 SK텔레콤의 제품에 포함하여 배포하려면 해당 오픈소스의 소스 코드의 공개가 필요합니다. 또한 이 오픈소스와 결합하는 SK텔레콤의 소스 코드까지도 동일한 오픈소스 라이선스를 적용하여 공개해야 합니다. 

따라서, _**Copyleft 라이선스 유형의 라이선스가 적용된 오픈소스는 SK텔레콤이 배포하는 제품에 포함하지 마세요.**_ 반드시 포함해야 하는 경우라면 TDE &gt; OSPO에 티켓을 생성하여 포함할 수 있는 방법을 문의하세요. 

Copyleft 라이선스 유형으로 분류할 수 있는 오픈소스 라이선스는 다음과 같습니다. 

* _BCL_
* [Creative Commons “Attribution-ShareAlike” \(CC BY-SA\) and “Attribution-NoDerivs” \(CC BY-ND\) licenses](http://creativecommons.org/licenses/)
* [GNU Classpath’s GPL + exception](http://www.gnu.org/software/classpath/license.html)
* [GNU GPL v1, v2, v3](http://opensource.org/licenses/gpl-license.php)
* [GNU LGPL v2.1, v3](http://opensource.org/licenses/lgpl-license.php) \(단, LGPL이 적용된 컴포넌트를 [dynamically-linked](https://opensource.google/docs/thirdparty/licenses/#LinkingRequirements) 형태로 사용할 경우, 자사 코드를 공개하지 않는 방식으로 사용할 수 있습니다.\).
* Netscape Public License [NPL 1.0](http://www.mozilla.org/MPL/NPL/1.0/) and [NPL 1.1](http://www.mozilla.org/MPL/NPL/1.1/)
* [OSL](http://opensource.org/licenses/osl-2.1.php)
* [QPL](http://opensource.org/licenses/qtpl.php)
* [Sleepycat License](http://opensource.org/licenses/sleepycat.php)

이와 같이 소스 코드 공개 의무를 요구하는 Copyleft 라이선스 하의 오픈소스를 포함하는 소프트웨어를 배포할 경우, 사용자에게 소스 코드를 직접 제공하거나, 사용자가 요청시 소스 코드를 제공하겠다는 서명 약정서를 제공해야 합니다. 이에 대한 세부 절차 및 방법은 다음 가이드를 참고하세요. 

{% page-ref page="../compliance.md" %}

## Weak Copyleft 라이선스 유형 

Weak copyleft 라이선스 유형은 Copyleft 라이선스 유형과 동일한 의무사항 준수를 요구하지만 한 가지 중요한 예외를 갖고 있습니다. Weak Copyleft 라이선스 유형의 라이브러리를 사용하여 소프트웨어를 배포할 경우, 해당 라이브러리의 소스 코드만 공개하면 됩니다 \(단, 해당 라이브러리의 수정사항은 공개 범위에 포함됩니다.\). 즉, GPL 등의 Copyleft 라이선스 유형과는 달리 Weak Coplyeft 라이선스 유형의 라이브러리를 사용하는 다른 소프트웨어는 동일한 라이선스로 소스 코드를 공개해야 할 의무가 없습니다. 

Weak Copyleft 라이선스 유형으로 분류할 수 있는 오픈소스 라이선스는 다음과 같습니다. 

* Common Development and Distribution License [CDDL 1.0](http://opensource.org/licenses/cddl1.php), _CDDL 1.1_
* _CeCILL-C License_
* [CPL 1.0](http://opensource.org/licenses/cpl1.0.php)
* [EPL 1.0](http://opensource.org/licenses/eclipse-1.0.php) and [EPL 2.0](https://opensource.org/licenses/EPL-2.0) \(Eclipse Public License\)
* [IPL 1.0](http://opensource.org/licenses/ibmpl.php) \(IBM Public License\)
* Mozilla Public License [MPL 1.0](http://opensource.org/licenses/mozilla1.0.php), [MPL 1.1](http://opensource.org/licenses/mozilla1.1.php), and [MPL 2.0](http://opensource.org/licenses/MPL-2.0)
* [Apple Public Source License \(APSL\) 2.0](http://opensource.org/licenses/apsl-2.0.php)
* _Ruby_

{% hint style="warning" %}
LGPL의 경우, Dynamic Link하여 사용할 경우, Weak Copyleft 라이선스 유형으로 간주하여 사용할 수 있습니다.
{% endhint %}

## Permissive  라이선스 유형

Permissive  라이선스 유형은 제한이 거의 없어서 상대적으로 준수하기가 쉬운 라이선스이며, 일반적으로 저작권 표시, 라이선스 고지 등의 고지 의무 준수를 요구하기 때문에 소프트웨어를 외부 배포 시에는 라이선스가 요구하는 고지를 해야 합니다. 

Permissive 라이선스로 분류할 수 있는 오픈소스 라이선스는 다음과 같습니다. 

* Academic Free License: [AFL 2.1](http://web.archive.org/web/20060428203736/http://opensource.org/licenses/afl-2.1.php) and [AFL 3.0](http://opensource.org/licenses/AFL-3.0)
* [Apache License 2.0](http://apache.org/licenses/LICENSE-2.0)
* [Artistic License 1.0](http://opensource.org/licenses/artistic-license-1.0) and [Artistic License 2.0](http://opensource.org/licenses/artistic-license-2.0)
* [ASL 1.1](http://apache.org/licenses/LICENSE-1.1) \(Apache Software License 1.1\)
* [Autodesk DWF Toolkit](http://usa.autodesk.com/adsk/servlet/item?siteID=123112&id=5522878)
* [Boost Software License](http://www.boost.org/users/license.html)
* [BSD \(occasionally referred to as the “University of California” license\)](https://opensource.org/licenses/bsd-license.php)
* [BSD 3-clause \(sometimes called BSD-new\)](https://opensource.org/licenses/BSD-3-Clause)
* [BSD + Patent](https://opensource.org/licenses/BSDplusPatent)
* [BSD - AES variant](https://web.archive.org/web/20190806093009/https://fedoraproject.org/wiki/Licensing:BSD#AES_Variant)
* [Creative Commons “Attribution” \(CC BY\) license](http://creativecommons.org/licenses/)
* _JSON License_ \(MIT license with the added note: “The Software shall be used for Good, not Evil.”\)
* [Eclipse Distribution License \(BSD variant\)](https://www.eclipse.org/org/documents/edl-v10.php)
* [FreeType Project License](http://freetype.sourceforge.net/FTL.TXT)
* [ISC License](http://opensource.org/licenses/ISC)
* [libjpeg-turbo](http://bazaar.launchpad.net/~tom-gall/libjpeg-turbo/trunk/view/1/README)
* [LibTIFF](http://www.remotesensing.org/libtiff/misc.html)
* [Lucent Public License 1.02 \(used by Plan 9 now, but different from “the Plan 9 license”\)](http://cm.bell-labs.com/plan9/license.html)
* [Microsoft Public License \(MS-PL\)](http://opensource.org/licenses/MS-PL)
* [MIT/X11/Expat](http://opensource.org/licenses/mit-license.php)
* [MIT adapted by CMU](https://web.archive.org/web/20190922104304/https://fedoraproject.org/wiki/Licensing:MIT?rd=Licensing/MIT#CMU_Style)
* [NCSA](http://opensource.org/licenses/UoI-NCSA.php)
* [OpenSSL](http://www.openssl.org/source/license.html)
* [PHP License 2.02](http://www.php.net/license/2_02.txt) and [3.0](http://www.php.net/license/3_0.txt)
* _PostgreSQL License_
* [Python Imaging Library \(PIL\) License](https://web.archive.org/web/20190921164759/http://www.pythonware.com/products/pil/license.htm)
* [TCP Wrappers](http://www.blackberry.com/support/blackberrypresenter/opensourcefiles/LICENSE-BSD-LIBWRAP.TXT)
* [Python Software Foundation](http://www.python.org/download/releases/2.3.2/license/)
* [STLport License](https://web.archive.org/web/20190804123932/http://www.stlport.org/doc/license.html)
* [TCP Wrappers](http://www.blackberry.com/support/blackberrypresenter/opensourcefiles/LICENSE-BSD-LIBWRAP.TXT)
* [Unicode, Inc. License Agreement - Data Files and Software](http://www.unicode.org/copyright.html#Exhibit1)
* [Universal Permissive License \(UPL\), Version 1.0](http://opensource.org/licenses/UPL)
* [W3C Software license](http://opensource.org/licenses/W3C.php)
* [X.Net](http://opensource.org/licenses/xnet.php)
* [Zend Engine License, v2.00](http://www.zend.com/license/2_00.txt)
* [zlib/libpng](http://opensource.org/licenses/zlib-license.php)
* [ZPL](http://opensource.org/licenses/zpl.php)

이와 같이 고지 의무를 요구하는 Permissive 라이선스 하의 오픈소스를 포함하는 소프트웨어를 배포할 경우, "저작권 표시", "라이선스 고지" 등의 의무를 준수해야 합니다. 예를 들어, SK텔레콤이 배포하는 모바일 애플리케이션은 요구되는 고지 사항을 "About" 페이지를 통해 제공할 수 있습니다. 

세부 절차는 다음 가이드를 참고하세요. 

{% page-ref page="../compliance.md" %}

## Public Domain 유형

Public Domain과 같이 아무런 제한 없이 무료로 사용할 수 있는 라이선스가 있습니다. 

* [Creative Commons CC0 \(public domain dedication\)](http://creativecommons.org/publicdomain/zero/1.0/)
* [qmail Terms of Distribution](http://cr.yp.to/qmail/dist.html)
* [Unlicense](http://unlicense.org/)

{% hint style="warning" %}
단, Public Domain이라고 선언하는 소프트웨어라도 사례별로 법적 검토가 필요한 복잡한 문제가 내재되어 있을 수 있습니다. 사용하려는 코드가 Public Domain인지 확인이 필요하다면 TDE &gt; OSPO에 티켓을 생성하여 문의하세요.
{% endhint %}

## 사용 불가 라이선스

아래와 같은 여러 이유로 일부 오픈소스 라이선스는 SK텔레콤의 제품에 사용하기에 적합하지 않은 조건을 포함하고 있습니다. 

### AGPL \(Affero GPL\)과 SSPL

AGPL \(GNU Affero General Public License\) 또는 SSPL \(Server Side Public Licese\)에 따라 공개된 오픈소스는 SK텔레콤의 제품에 사용할 수 없습니다. 자세한 사항은 다음 페이지를 참고하세요. 

{% page-ref page="agpl.md" %}

### 비상업 라이선스

연구, 학습만을 위해서라고 해도 SK텔레콤 내에서 사용한다면 상업적인 활동으로 간주될 수 있습니다. 따라서 비상업적으로만 사용할 수 있도록 제한하는 라이선스에 따라 공개된 오픈소스는 SK텔레콤에서 사용할 수 없습니다. 이러한 비상업용 \(Non-Commercial\) 라이선스는 다음과 같습니다.

* CC BY-NC
* CC BY-NC-SA
* CC BY-NC-ND

### 이외 언급되지 않은 라이선스

위에서 분류되지 않은 라이선스가 적용된 오픈소스를 SK텔레콤의 제품에 사용하기 위해서는 OSPO의 검토가 필요합니다. TDE &gt; OSPO에 티켓을 생성하여 문의하세요.



{% hint style="success" %}
이 페이지는 다음 문서를 참고하였습니다. 

* [https://opensource.google/docs/thirdparty/licenses/](https://opensource.google/docs/thirdparty/licenses/)
* [https://verizonmedia.github.io/oss-guide/docs/using/using.html](https://verizonmedia.github.io/oss-guide/docs/using/using.html)
{% endhint %}

