---
description: contibute
---

# 기여하기

오픈소스는 소프트웨어를 개발할 때 가장 필수적인 구성요소가 되었습니다. 기업들은 오픈소스를 사용하여 제품 및 서비스를 구축하는 것에 그치지 않고, 오픈소스 프로젝트에 기여하는 전략적 가치도 고려하고 있습니다. 

그러나 오픈소스 프로젝트와 커뮤니티에 대한 이해와 전략 없이 뛰어들면 실망감만 안겨줄 수 있습니다. 특히, 커뮤니티에서 기업의 명성이 떨어질 뿐만 아니라 법적 위험이 발생할 수도 있습니다. 

이 가이드에서는 기업이 오픈소스에 기여하는 이유 및 방법에 대해 설명합니다. 

## 기여에 앞서

### 오픈소스에 기여해야 는 이유

{% page-ref page="expect.md" %}

### 오픈소스 프로젝트 관리 구조

오픈소스 프로젝트를 구성하는 인원의 역할과 책임은 어떻게 되나요?

{% page-ref page="role.md" %}

### 오픈소스 기여 형태

오픈소스에 기여하는 유형에는 어떤 것들이 있나요?

{% page-ref page="type.md" %}

### 좋은 기여자가 되려면

{% page-ref page="good.md" %}

### 프로젝트 체크

{% page-ref page="validate.md" %}

이제 기여 방법과 절차에 대해 세부적으로 알아보겠습니다. 

기여 프로세스는 오픈소스 프로젝트마다 다릅니다. 

{% hint style="success" %}
* 프로젝트마다 코딩 스타일, language, formatting, bug/ticket 관리, 릴리즈 시기 등에 대한 다양한 가이드라인을 갖고 있습니다. 
* 어떤 프로젝트는 Contributor Agreement를 요구하는 반면, 어떤 프로젝트는 Signed-off-by나 다른 형태의 요구를 합니다. 
* Patch를 받는 방식도 요즘은 대부분 Github의 Pull Request로 받지만, 어떤 프로젝트는 여전히 Mailing List를 이용하기도 합니다. 
{% endhint %}

## 1. 문서 읽기

그렇기 때문에 기여하고자 하는 프로젝트의 프로세스를 제대로 이해하기 위해서는 우선 프로젝트에서 제공하는 문서를 봐야 합니다. 대개의 프로젝트는 CONTRIBUTING 또는 README 파일로 이러한 문서를 제공합니다.

{% hint style="info" %}
예를 들어, Kubernates는 기여자를 위한 가이드를 자세히 제공합니다. 

* [contributing.md](https://github.com/kubernetes/community/blob/master/contributors/guide/contributing.md) : Kubernates에 기여하기 위한 가이드
* [github\_workflow.md](https://github.com/kubernetes/community/blob/master/contributors/guide/github-workflow.md) : GitHub에서 기여하기 위한 절차 설명
{% endhint %}

## 2. 기여 제출하기

문서에서 알려주는 프로세스에 따라 기여를 제출합니다. 이때 몇가지 알고 있으면 좋은 사항들을 소개합니다.

### 효과적인 커뮤니케이션 방법

{% page-ref page="undefined.md" %}

### 과거 자료 수집

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

{% hint style="info" %}
Issue에 대한 커뮤니케이션 Tip 

1. 당신이 다루고자 하는 오픈된 Issue가 있다면, 먼저 comment를 남겨서 다른 사람들이 중복으로 작업하지 않게 하세요. 
2. 오래전에 오픈된 Issue라면, 이미 해결된 것일 수 있습니다. 작업을 시작하기 전에 comment로 해결이 된 것은 아닌지 확인하세요. 
3. 당신이 Issue를 오픈했지만, 나중에 스스로 답을 알아낸 경우, 해당 Issue에 대한 답을 다른 사람도 알 수 있도록 comment를 작성하고 이슈를 close 하세요. 이렇게 문서화하는 것조차도 프로젝트에 기여하는 것입니다. 
{% endhint %}

### Pull Request

Pull Request를 통해 기여를 제출하는 방법은 다음 페이지를 참고합니다. 



일반적으로 다음 상황에서 Pull Request를 오픈합니다. 

* 사소한 수정 사항 제출 \(예: 오타, 링크 오류 등\)
* Issue에서 이미 논의가 된 사항에 대한 작업 시작

Pull Request는 작업이 완료된 이후에 해야 하는 것은 아닙니다. 일반적으로 Pull Request를 일찍 오픈하여 다른 사람들의 피드백을 받는 게 좋습니다. 제목 줄에 "WIP" \(Work in Progress\)라고 표시하여 아직 진행 중인 작업이라고 표시하고, 나중에 언제든지 더 많은 Commit을 추가할 수 있습니다. 

GitHub에 있는 프로젝트라면 Pull Request를 제출 시 다음 사항을 참고할 수 있습니다. 

<table>
  <thead>
    <tr>
      <th style="text-align:left">&#xBC29;&#xBC95;</th>
      <th style="text-align:left">&#xC124;&#xBA85;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Repository Fork</td>
      <td style="text-align:left">
        <p>Repository&#xB97C; <a href="https://guides.github.com/activities/forking/">Fork</a>&#xD558;&#xACE0;
          Local PC&#xC5D0; &#xBCF5;&#xC81C;(Clone)&#xD569;&#xB2C8;&#xB2E4;. &#xC774;&#xB85C;&#xC368;
          &#xB2F9;&#xC2E0;&#xC758; Local PC&#xAC00; Original &quot;Upstream&quot;
          repository&#xC640; &#xC6D0;&#xACA9;&#xC73C;&#xB85C; &#xC5F0;&#xACB0;&#xB429;&#xB2C8;&#xB2E4;.</p>
        <p>&quot;Upstream&quot;&#xC758; &#xBCC0;&#xACBD; &#xC0AC;&#xD56D;&#xC744;
          &#xC218;&#xC2DC;&#xB85C; &#xB2F9;&#xACA8;&#xC640;&#xC11C; (Pull) &#xD56D;&#xC0C1;
          &#xCD5C;&#xC2E0; &#xC0C1;&#xD0DC;&#xB97C; &#xC720;&#xC9C0;&#xD569;&#xB2C8;&#xB2E4;.
          &#xC774;&#xB294; &#xB098;&#xC911;&#xC5D0; &#xB2F9;&#xC2E0;&#xC758; &#xBCC0;&#xACBD;
          &#xC0AC;&#xD56D;&#xC744; Merge &#xD560; &#xB54C; Conflict &#xB418;&#xB294;
          &#xAC78; &#xC904;&#xC5EC;&#xC90D;&#xB2C8;&#xB2E4;.</p>
        <p>&#xC790;&#xC138;&#xD55C; &#xC0AC;&#xD56D;&#xC740; &#xB2E4;&#xC74C; &#xC548;&#xB0B4;&#xB97C;
          &#xCC38;&#xACE0;&#xD558;&#xC138;&#xC694;. &quot;<a href="https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork">Syncing a fork</a>&quot;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Branch &#xC0DD;&#xC131;</td>
      <td style="text-align:left">&#xBCC4;&#xB3C4;&#xC758; <a href="https://guides.github.com/introduction/flow/">Branch&#xB97C; &#xC0DD;&#xC131;</a>&#xD558;&#xC5EC;
        &#xC218;&#xC815; &#xC791;&#xC5C5;&#xC744; &#xD569;&#xB2C8;&#xB2E4;.</td>
    </tr>
    <tr>
      <td style="text-align:left">PR&#xC5D0; &#xAD00;&#xB828; Issue &#xBC88;&#xD638; &#xCD94;&#xAC00;</td>
      <td
      style="text-align:left">PR (Pull Request) &#xC624;&#xD508; &#xC2DC;, &#xAD00;&#xB828;&#xB41C;
        Issue&#xC758; &#xBC88;&#xD638;&#xB098; &#xCC38;&#xC870;&#xD558;&#xB294;
        &#xBB38;&#xC11C;&#xB97C; &#xD45C;&#xC2DC;&#xD558;&#xC138;&#xC694;. (&#xC608;:
        &quot;Closes #37&quot;)</td>
    </tr>
    <tr>
      <td style="text-align:left">&#xC804;&#xD6C4; &#xC2A4;&#xB0C5;&#xC0F7; &#xCD94;&#xAC00;</td>
      <td style="text-align:left">&#xB2F9;&#xC2E0;&#xC758; &#xC218;&#xC815; &#xC0AC;&#xD56D;&#xC774; HTML/CSS&#xB97C;
        &#xBCC0;&#xACBD;&#xD558;&#xC600;&#xB2E4;&#xBA74;, Pull Request&#xC5D0;
        &#xC804;&#xD6C4; &#xC2A4;&#xB0C5;&#xC0F7; &#xC774;&#xBBF8;&#xC9C0;&#xB97C;
        &#xCD94;&#xAC00;&#xD558;&#xC138;&#xC694;.</td>
    </tr>
    <tr>
      <td style="text-align:left">&#xC218;&#xC815; &#xC0AC;&#xD56D; &#xD14C;&#xC2A4;&#xD2B8;</td>
      <td style="text-align:left">&#xC218;&#xC815; &#xC0AC;&#xD56D;&#xC744; &#xBC18;&#xC601;&#xD558;&#xC5EC;
        &#xAE30;&#xC874; &#xD14C;&#xC2A4;&#xD2B8;&#xB97C; &#xC2E4;&#xD589;&#xD558;&#xC138;&#xC694;.
        &#xD544;&#xC694;&#xD560; &#xACBD;&#xC6B0; &#xC0C8;&#xB85C;&#xC6B4; &#xD14C;&#xC2A4;&#xD2B8;
        &#xCF00;&#xC774;&#xC2A4;&#xB97C; &#xC791;&#xC131;&#xD558;&#xC138;&#xC694;.
        &#xC5B4;&#xB290; &#xACBD;&#xC6B0;&#xB77C;&#xB3C4; &#xC218;&#xC815; &#xC0AC;&#xD56D;&#xC774;
        &#xAE30;&#xC874; &#xD504;&#xB85C;&#xC81D;&#xD2B8;&#xB97C; &#xC190;&#xC0C1;&#xC2DC;&#xCF1C;&#xC11C;&#xB294;
        &#xC548; &#xB429;&#xB2C8;&#xB2E4;.</td>
    </tr>
    <tr>
      <td style="text-align:left">&#xD504;&#xB85C;&#xC81D;&#xD2B8; &#xC2A4;&#xD0C0;&#xC77C; &#xC720;&#xC9C0;</td>
      <td
      style="text-align:left">&#xB4E4;&#xC5EC;&#xC4F0;&#xAE30; (Indent), &#xC138;&#xBBF8;&#xCF5C;&#xB860;,
        &#xB610;&#xB294; &#xC8FC;&#xC11D; &#xB4F1;&#xC744; &#xD504;&#xB85C;&#xC81D;&#xD2B8;
        &#xC2A4;&#xD0C0;&#xC77C;&#xB300;&#xB85C; &#xB530;&#xB974;&#xC138;&#xC694;.
        &#xADF8;&#xB798;&#xC57C; Maintainer&#xAC00; Merge &#xD558;&#xAE30; &#xC27D;&#xACE0;,
        &#xB098;&#xC911;&#xC5D0; &#xB2E4;&#xB978; &#xC0AC;&#xB78C;&#xB4E4;&#xC774;
        &#xC774;&#xD574;&#xD558;&#xACE0; &#xC720;&#xC9C0;&#xD558;&#xAE30; &#xC218;&#xC6D4;&#xD569;&#xB2C8;&#xB2E4;.</td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
Pull Request가 처음이라면 [Make a Pull Request](http://makeapullrequest.com/)\(비디오 강의\)를 참고하세요.  또한, [First Contributions](https://github.com/Roshanjossey/first-contributions) 에서 Pull Request 만드는 것을 연습할 수 있습니다. 
{% endhint %}

## 3. Feedback 받기

기여를 제출하면 이에 대한 Feedback을 받게 됩니다. 

{% hint style="warning" %}
일반적으로 Feedback은 개선이나 변경 사항이 어떤 방식으로 동작하는지, 왜 그런 방식을 채택하였는지 등에 대한 설명을 요구합니다. 이 Feedback은 때로는 대응하기 어려울 수도 있지만, 기여의 수준을 높이는 과정이라고 받아들이는 것이 좋습니다.
{% endhint %}

Feedback은 보통 다음 세 가지 중 하나에 해당합니다.

### \(1\) 응답이 없다? 

기여하기 전에 프로젝트가 활발한지 먼저 [확인](https://opensource-skt.gitbook.io/guide/contribute/validate)하는 게 좋습니다. 어느 정도 활발한 프로젝트에서도 기여에 대해 응답을 받지 못할 수도 있습니다. 

일주일 이상 응답을 받지 못한 경우, 동일한 스레드에 정중하게 누군가에게 검토를 요청하는 것이 좋습니다. 적절한 사람의 이름을 알고 있다면 @-멘션 기능을 이용하세요. 

{% hint style="danger" %}
단, 개인적으로 연락하지는 마세요. 오픈소스 프로젝트에서 공개 커뮤니케이션은 필수입니다. 
{% endhint %}

그럼에도 여러 가지 이유가 있겠지만 아무도 반응하지 않을 수도 있습니다. 썩 좋은 기분은 아니지만 낙담할 필요는 없습니다. 이는 누구에게나 일어날 수 있는 일입니다. 기여할 수 있는 다른 방법이나 다른 프로젝트를 찾아보세요. 

### \(2\) 수정을 요청한다?

아이디어에 대한 설명이나 코드를 수정하라는 요청을 받는 것은 일반적입니다. 이렇게 누군가 수정을 요청했다면 바로 응답하세요. 그는 자기 시간을 내서 당신의 기여를 검토했습니다. 

PR을 오픈한 상태로 응답하지 않고 남겨두는건 결례입니다. 더 이상 문제를 해결할 여건이 아닌 경우라면, Maintainer에게 더 진행할 수 없다고 알리세요. 그렇게 PR을 Close 하거나 다른 사람이 인수하여 추가로 진행할 수도 있습니다. 

### \(3\) 거절됐다?

당신의 기여는 결국 수락될 수도 있고, 수락되지 않을 수도 있습니다. 수락되지 않은 이유가 잘 이해되지 않을 경우, Maintainer에게 설명을 요청하는 것도 합리적입니다. 그러나 이것이 그들의 결정임을 존중해야 합니다. 논쟁하거나 적대적으로 행동하지 마세요. 끝까지 이견이 조율되지 않으면, 당신은 언제든지 Fork 하여 자신의 프로젝트에 작업할 수 있습니다. 

{% hint style="warning" %}
코드가 승인되기까지 여러 차례의 반복적인 수정 과정을 거쳐야 할 수도 있으며, 때에 따라서는 거부될 수도 있습니다. 이때는 낙심하거나 포기하기보다는 거부된 이유에 대해 자세히 알아보고, 다음 기여가 향상되는 기회로 삼는 것이 좋습니다.
{% endhint %}

### \(4\) 수락됐다!

축하합니다! 드디어 오픈소스 기여에 성공했습니다.

