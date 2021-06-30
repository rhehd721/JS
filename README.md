# JS

## 문법
```js
var 갑을 = "병정";
var Früh = "foobar"; // Früh: 독일어로 "이른"
```

## 선언
- var
    - 변수를 선언. 추가로 동시에 값을 초기화.
- let
    - 블록 범위(scope) 지역 변수를 선언. 추가로 동시에 값을 초기화.
- const
    - 블록 범위 읽기 전용 상수를 선언.

## 변수 할당
```js
 var a;
console.log("a 값은 " + a); // "a 값은 undefined"로 로그가 남음.

console.log('b 값은 ' + b); // b 값은 undefined
var b;

console.log("c 값은 " + c); // ReferenceError 예외 던짐

let x;
console.log('x 값은 ' + x); // x 값은 undefined

console.log('y 값은 ' + y); // ReferenceError 예외 던짐
let y;
```
- 값이 할당 되었는지 확인
```js
var input;
if(input === undefined) {   // True
  doThis();
} else {
  doThat();
}
```
- 전역변수, 지역변수
```js
if (true) {
  var x = 5;
}
console.log(x); // 5

if (true) {
  let y = 5;
}
console.log(y); // ReferenceError: y is not defined
```
