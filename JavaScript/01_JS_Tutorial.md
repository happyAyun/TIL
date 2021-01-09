# 01. JS_Tutorial

< Where to >

- html 문서에 `< script > ... </ script >` 를 작성한 하고, `... `부분에 javascript 언어를 넣어준다.
  -  `< script src="..."> </ script >`  : `...`부분에 javascript.js의 파일 위치를 넣어주면 연동된다.

---

< Output >

- `document.getElementIdBy("id")` : html문서에서 id와 같은 id를 가진 부분을 가리킴.
  - `document.getElementIdBy("id").innerHTML="hi~"` : id라는 부분에 hi~ 의 html  요소를 정의함.

- `document.write();` : HTML화면에 문자열 출력. 테스트의 목적으로 간단히 사용함.
  - 수의 계산은 () , 문자열의 출력은 ("")
- `window.alert();`  => window생략 가능 => `alert();` : 경고(안내)창이 열림.
- `console.log` : 디버깅의 목적으로 사용된다.
- `window.print()` : 현재의 페이지를 프린트하기 위한 브라우저가 열린다.

---

< Comments >

- 주석 처리 :  `//`, `/* */`

---

< Variables >

- `문자(열) + 숫자`  => `문자열 + 문자열` 로 변화된다. 

```javascript
var x = "5" + 2 + 3; // 앞이 문자열이므로 2,3도 문자로 인식
// x = 523

var x = 2 + 3 + "5"; // 앞이 숫자이고, 뒤가 문자이므로 
// 2+3 은 숫자로 인식해 덧셈을 통하여 5가 되고
// 뒤는 문자열 5이므로 문자열+문자열이 되어 
// x = 55
```

---

< Operators >

`===` : 값(value) 도 같고, 타입(type) 도 같다. (AND)

`!==` : 값(value) 이 같지 않거나, 타입(type) 이 같지 않다. (OR)

`? :` : 삼항 연산자

```
(조건) ? 조건이 참일 경우 : 거짓일 경우
```

`<<` : Zero fill left shift

`>>` : Signed right shift

`>>>` : Zero fill right shift

---

< Arithmetic >

-  `Math.pow(연산할 수(x),x의 n제곱의 수)` :`Math.pow(x,2)` = x^2

- `person.name` = `person["name"]`
- `typeof` : `typeof 변수`

---

< Data Types >

- Primitive Data
  - `number`
  - `string`
  - `boolean` - true, false
  - `undefined`

---

- Complex Data
  - `object` - { }
  - `function`

---

- `arrays` - [ ]

- `null`

  ```javascript
  typeof undefined           // undefined
  typeof null                // object
  
  null === undefined         // false - type이 다름.
  null == undefined          // true - 값이 없다는 건 같다.
  ```

---

