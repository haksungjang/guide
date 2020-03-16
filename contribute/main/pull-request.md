---
description: Pull Request와 GitHub 사례를 소개합니다.
---

# Pull Request

## Pull Request 시기

일반적으로 다음 상황에서 Pull Request를 오픈합니다. 

* 사소한 수정 사항 제출 \(예: 오타, 링크 오류 등\)
* Issue에서 이미 논의가 된 사항에 대한 작업 시작

Pull Request는 작업이 완료된 이후에 해야 하는 것은 아닙니다. 일반적으로 Pull Request를 일찍 오픈하여 다른 사람들의 피드백을 받는 게 좋습니다. 제목 줄에 "WIP" \(Work in Progress\)라고 표시하여 아직 진행 중인 작업이라고 표시하고, 나중에 언제든지 더 많은 Commit을 추가할 수 있습니다. 

## GitHub 사례

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
</table>{% hint style="warning" %}
Pull Request가 처음이라면 [Make a Pull Request](http://makeapullrequest.com/)\(비디오 강의\)를 참고하세요.  또한, [First Contributions](https://github.com/Roshanjossey/first-contributions) 에서 Pull Request 만드는 것을 연습할 수 있습니다. 
{% endhint %}

{% hint style="warning" %}
참고로, Kubernates는 다음과 같은 Github workflow에 대한 설명 문서를 제공합니다.

* [github\_workflow.md](https://github.com/kubernetes/community/blob/master/contributors/guide/github-workflow.md) : GitHub에서 기여하기 위한 절차 설명
{% endhint %}

