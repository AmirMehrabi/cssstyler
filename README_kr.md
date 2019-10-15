## 고지사항 ##

fork된 저장소입니다. [메인 저장소](https://github.com/senchalabs/cssbeautify).


# CSS Beautify #

CSS Beautify는 [CSS](http://www.w3.org/Style/CSS/) 문서를 들여쓰기 및 포맷해주는 Javascript 구현체입니다.

CSS 구문이 다음과 같이 주어지면

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify로 처리된 예시는 다음과 같습니다.

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

[cssbeautify.com](http://cssbeautify.com)에서 데모를 확인할 수 있습니다.
명령줄(CLI)에서 사용하려면 Node.js [cssbeautify](https://npmjs.org/package/cssbeautify)를 설치하세요.

더 많은 예제는 [테스트 스위트](http://cssbeautify.com/test/)를 통해 확인하세요.

## cssbeautify() 함수 사용 ##

CSS Beautify는 순수(바닐라) JavaScript로 쓰여셨으므로, JavaScript 코드 어디에서든 실행할 수 있습니다.

API는 매우 간단합니다.

```javascript
var result = cssbeautify(style, options);
```

**options**은 포맷 형식 옵션 객체입니다. 사용할 수 있는 옵션은 다음과 같습니다.

  *  <code>indent</code> 는 들여쓰기에 사용할 문자열입니다 (기본값 공백문자 4개입니다.)
  *  <code>openbrace</code> 는 중괄호 시작 문자('{') 배치 위치를 결정합니다. *end-of-line* (기본값) 또는 *separate-line*을 지정할 수 있습니다.
  *  <code>autosemicolon</code> 는 마지막 ruleset 뒤에 반드시 세미콜론(쉼표)를 넣습니다, (기본값은 *false*)

호출 예제:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## 기여 ##

기여 환영입니다! [기여 가이드](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md)에서 자세히 알아보세요.

## 라이센스 ##

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

이 소프트웨어의 복제본과 관련된 문서화 파일(“소프트웨어”)을 획득하는 사람은 누구라도 
소프트웨어를 별다른 제한 없이 무상으로 사용할 수 있는 권한을 부여 받는다. 
여기에는 소프트웨어의 복제본을 무제한으로 사용, 복제, 수정, 병합, 공표, 배포, 
서브라이선스 설정 및 판매할 수 있는 권리와 
이상의 행위를 소프트웨어를 제공받은 다른 수취인들에게 허용할 수 있는 권리가 포함되며, 
다음과 같은 조건을 충족시키는 것을 전제로 한다.

위와 같은 저작권 안내 문구와 본 허용 문구가 소프트웨어의 모든 복제본 및 중요 부분에 포함되어야 한다.
이 소프트웨어는 상품성, 특정 목적 적합성, 그리고 비침해에 대한 보증을 포함한 
어떠한 형태의 보증도 명시적이나 묵시적으로 설정되지 않은 “있는 그대로의” 상태로 제공된다.

소프트웨어를 개발한 프로그래머나 저작권자는 어떠한 경우에도 소프트웨어나 
소프트웨어의 사용 등의 행위와 관련하여 일어나는 어떤 요구사항이나 손해 및 기타 책임에 대해 
계약상, 불법행위 또는 기타 이유로 인한 책임을 지지 않는다.
