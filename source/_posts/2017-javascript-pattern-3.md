---
title: '자바스크립트 패턴 3주'
date: 2017-04-24 10:40:51
categories:
- 2017 스터디
- 자바스크립트 패턴
tags:
- 2017_상반기_스터디
- 자바스크립트
thumbnail: https://github.com/youngbeomrhee
---
### ▶ 자바스크립트 최적화 패턴
- [최적화 패턴 예제 소스](https://github.com/youngbeomrhee/jssample/tree/master/javacafe_2017_frontend/ch003)

---

### ▶ 스터디 진행 시, 모호했던 부분 내용 정리
- var로 선언한 전역변수는 삭제가 안되고 암묵적 전역으로 선언된 변수만 삭제된 경우 ?
{% blockquote %}
기본적으로 프로퍼티만이 삭제 가능하고, 변수는 삭제가 안됩니다. 암묵적 전역변수는 삭제 가능한 것으로 봐서 온전한 변수라기 보다는 전역객체의 프로퍼티로 할당된다고 볼 수 있습니다.
{% endblockquote %}
- new Function으로 선언한 코드의 실행환경 ?
{% blockquote %}
_**"Function 생성자로 만든 함수는 그들의 생성 문맥(context)에 클로저(closure)를 만들지 않고 항상 전역 범위(global scope)로 생성됩니다. 그들을 실행할 때, 함수는 Function 생성자가 호출됐던 범위가 아니라 오직 자신의 지역 변수 및 전역 변수에만 액세스할 수 있습니다."**_ 라고 [MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Function)에 명시되어 있네요. 어떻게 그렇게 실행되는지는 감춰져 있어 확인이 어렵습니다. 'new Function'으로 선언한 경우에는 선언위치와 상관없이 전역에서 실행한 것과 같다고 이해하면 될 것 같습니다.
{% endblockquote %}

---
 2017년 4월 22일에 진행한 자료입니다. 질문사항이 있으시면 댓글로 남겨주시길 바랍니다:)
