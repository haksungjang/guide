# 기여 절차와 방법

사실 오픈소스 프로젝트마다 요구하는 절가 각기 다릅니다. 

{% hint style="warning" %}
* 프로젝트마다 코딩 스타일, language, formatting, bug/ticket 관리, 릴리즈 시기 등에 대한 다양한 가이드라인을 갖고 있습니다. 
* 어떤 프로젝트는 Contributor Agreement를 요구하는 반면, 어떤 프로젝트는 Signed-off-by나 다른 형태의 요구를 합니다. 
* Patch를 받는 방식도 요즘은 대부분 Github의 Pull Request로 받지만, 어떤 프로젝트는 여전히 Mailing List를 이용하기도 합니다. 
{% endhint %}

그렇기 때문에 기여하고자 하는 프로젝트의 프로세스를 제대로 이해하기 위해서는 우선 프로젝트에서 제공하는 문서를 봐야 합니다. 

## 0. 기본 규칙

### 회사 이메일 사용

sktelecom.com 이메일을 사용해서 기여하세요. GitHub에 있는 프로젝트에 기여할때는 다음 페이지를 참고하여 이메일을 설정할 수 있습니다. : [How to associate your commit with a sktelecom.com email](https://help.github.com/articles/setting-your-email-in-git/).

### 저작권 표시

AUTHORS 파일과 소스 코드 파일에 저작권 정보 \(SK TELECOM CO., LTD.\)를 표기하여 SK텔레콤이 기여에 대한 저작권 등 소유권을 주장할 수 있음을 표시하세요. 

### OSPO에 알림

새로운 프로젝트에 처음 기여할때에는 먼저 OSPO에 알려주시기 바랍니다. \(T-DE &gt; OSPO 에서 Ticket 생성\) \(haksung : 방법 구체화하여 추가 필요\)

## 1. 문서 읽기

대개의 프로젝트는 CONTRIBUTING 또는 README 파일로 이러한 문서를 제공합니다. 

{% hint style="warning" %}
예를 들어, Kubernetes는 기여자를 위한 자세한 가이드를 제공합니다. 

* [contributing.md](https://github.com/kubernetes/community/blob/master/contributors/guide/contributing.md) : Kubernetes에 기여하기 위한 가이드
{% endhint %}

문서에서 요구하는 사항을 잘 준수할수록 당신의 기여가 수락될 가능성이 커집니다. 

## 2. CLA \(Contributors License Agreement\) 검토하기 

어떤 프로젝트는 기여자에게 CLA \(Contributor License Agreement\)에 서명할 것을 요구합니다. 이때 CLA에 임의로 서명하지 마세요. 이 경우는 OSPO의 승인을 받아야 합니다. T-DE &gt; OSPO 에서 Ticket을 생성하세요. \(haksung : OSPO 승인 절차 추가 필요\)

대부분의 CLA는 서명해도 문제가 되지 않기 때문에 승인 절차가 오래 걸리지 않습니다. 드문 경우지만, CLA에서 지적 재산권을 완전히 양도할 것을 요구하기도 합니다. 이럴 때는 CLA에 서명할 수 없습니다. 따라서 그 프로젝트에는 기여할 수 없습니다. 

## 3. 기여물 검토하기 

기여를 제출하기 전에 다음 사항을 한번 확인하세요.

* 기여할 권리가 있는 코드인가요? 당신이 작성한 코드라면 문제 되지 않습니다. 만약 기여하려는 코드에 당신이 작성하지 않은 코드가 포함되었다면 기여할 권리가 있는지 확인이 필요합니다. Jira Ticket을 생성하여 OSPO에 문의하세요. \(haksung : Jira Ticket 생성 방법 추가 제공 필요\)
* 회사의 민감하거나 독점적인 정보가 노출될 수 있는 코드를 제공하지 마세요.
* 기여하려는 코드에 특허가 포함되어 있나요? Jira Ticket을 생성하여 OSPO에 문의하세요. 

이외에 어떤 사항이라도 궁금한 사항이 있다면 Jira Ticket을 열고 OSPO에 문의하세요.

## 4. 기여 제출하기

이제 프로젝트의 문서에서 요구하는 절차에 따라 기여를 제출합니다. 일반적인 오픈소스 프로젝트에 기여하는 방법과 절차는 아래를 참고하세요. 

### 효과적인 커뮤니케이션 방법

{% page-ref page="communication.md" %}

### 과거 자료 확인 

무엇이든 시작하기 전에 먼저 이전에  다뤄진 적이 있는지 과거 자료를 확인하세요. 프로젝트의 README, 이슈, 메일링 리스트를 살펴보세요. 모든 문서를 다 확인할 필요 없이, 몇 가지 키워드를 검색하면 쉽게 확인할 수 있습니다. 

과거 자료에서 관련 내용을 찾을 수 없다면 이슈를 열거나 Pull Request를 통해 커뮤니키이션을 시작할 단계입니다. GitHub에서는 Issues와 Pull Request 기능을 제공합니다.

* Issues : 대화나 토론을 시작할 수 있습니다. 
* Pull Request : 문제에 대한 솔루션을 기여합니다. 

Issue 또는 Pull Request를 열기 전에 프로젝트가 제공하는 문서 \(일반적으로 CONTRIBUTING 또는 README\)를 확인하여 기여 절차 및 방법을 확인하세요. 예를 들어 특정 템플릿을 따르도록 요구하거나, 사전 테스트를 요구할 수 있습니다. 

기여를 위한 작업을 시작하기 전에 먼저 Issues를 오픈해서 커뮤니티 구성원에게 먼저 어떤 작업을 하려고 하는지 알리는 것도 좋은 방법입니다. 때에 따라 불필요한 작업을 진행하지 않도록 도움을 받을 수 있습니다. 

### Issue 오픈하기

일반적으로 다음 상황에서 Issue를 오픈합니다. 

* 스스로 해결할 수 없는 오류 보고
* 새로운 기능 또는 아이디어 제안
* 커뮤니티 비전, 또는 정책에 대한 토론

{% hint style="warning" %}
Issue에 대한 커뮤니케이션 Tip 

1. 당신이 다루고자 하는 오픈된 Issue가 있다면, 먼저 comment를 남겨서 다른 사람들이 중복으로 작업하지 않게 하세요. 
2. 오래전에 오픈된 Issue라면, 이미 해결된 것일 수 있습니다. 작업을 시작하기 전에 comment로 해결이 된 것은 아닌지 확인하세요. 
3. 당신이 Issue를 오픈했지만, 나중에 스스로 답을 알아낸 경우, 해당 Issue에 대한 답을 다른 사람도 알 수 있도록 comment를 작성하고 이슈를 close 하세요. 이렇게 문서화하는 것조차도 프로젝트에 기여하는 것입니다. 
{% endhint %}

### Pull Request

기여할 파일이 모두 준비가 되다면, Pull Request를 통해 기여를 제출하세요. Pull Request 방법은 다음 페이지를 참고하세요. 

{% page-ref page="pull-request.md" %}

## 3. Feedback 받기

기여를 제출하면 프로젝트로부터 Feedback을 받게 됩니다. 

{% hint style="warning" %}
일반적으로 Feedback은 개선이나 변경 사항이 어떤 방식으로 동작하는지, 왜 그런 방식을 채택하였는지 등에 대한 설명을 요구합니다. 이 Feedback은 때로는 대응하기 어려울 수도 있지만, 기여의 수준을 높이는 과정이라고 받아들이는 것이 좋습니다.
{% endhint %}

Feedback은 보통 다음 네 가지 중 하나에 해당합니다.

### 1\) 응답이 없다? 

기여하기 전에 프로젝트가 활발한지 먼저 [확인](https://opensource-skt.gitbook.io/guide/contribute/validate)하는 게 좋습니다. 어느 정도 활발한 프로젝트에서도 기여에 대해 응답을 받지 못할 수도 있습니다. 

일주일 이상 응답을 받지 못한 경우, 동일한 스레드에 정중하게 누군가에게 검토를 요청하는 것이 좋습니다. 적절한 사람의 이름을 알고 있다면 @-멘션 기능을 이용하세요. 

{% hint style="danger" %}
단, 개인적으로 연락하지는 마세요. 오픈소스 프로젝트에서 공개 커뮤니케이션은 필수입니다. 
{% endhint %}

그럼에도 여러 가지 이유가 있겠지만 아무도 반응하지 않을 수도 있습니다. 썩 좋은 기분은 아니지만 낙담할 필요는 없습니다. 이는 누구에게나 일어날 수 있는 일입니다. 기여할 수 있는 다른 방법이나 다른 프로젝트를 찾아보세요. 

### 2\) 수정을 요청한다?

아이디어에 대한 설명이나 코드를 수정하라는 요청을 받는 것은 일반적입니다. 이렇게 누군가 수정을 요청했다면 바로 응답하세요. 그는 자기 시간을 내서 당신의 기여를 검토했습니다. 

PR을 오픈한 상태로 응답하지 않고 남겨두는건 결례입니다. 더 이상 문제를 해결할 여건이 아닌 경우라면, Maintainer에게 더 진행할 수 없다고 알리세요. 그렇게 PR을 Close 하거나 다른 사람이 인수하여 추가로 진행할 수도 있습니다. 

### 3\) 거절됐다?

당신의 기여는 결국 수락될 수도 있고, 수락되지 않을 수도 있습니다. 수락되지 않은 이유가 잘 이해되지 않을 경우, Maintainer에게 설명을 요청하는 것도 합리적입니다. 그러나 이것이 그들의 결정임을 존중해야 합니다. 논쟁하거나 적대적으로 행동하지 마세요. 끝까지 이견이 조율되지 않으면, 당신은 언제든지 Fork 하여 자신의 프로젝트에 작업할 수 있습니다. 

{% hint style="warning" %}
코드가 승인되기까지 여러 차례의 반복적인 수정 과정을 거쳐야 할 수도 있으며, 때에 따라서는 거부될 수도 있습니다. 이때는 낙심하거나 포기하기보다는 거부된 이유에 대해 자세히 알아보고, 다음 기여가 향상되는 기회로 삼는 것이 좋습니다.
{% endhint %}

### 4\) 수락됐다!

축하합니다! 드디어 오픈소스 기여에 성공했습니다.

{% hint style="success" %}
이 페이지는 다음 문서를 참고하였습니다. 

* [https://todogroup.org/guides/participating/](https://todogroup.org/guides/participating/)
* [https://opensource.guide/how-to-contribute/](https://opensource.guide/how-to-contribute/)
* [https://verizonmedia.github.io/oss-guide/docs/contributing/contributing.html](https://verizonmedia.github.io/oss-guide/docs/contributing/contributing.html)
{% endhint %}

