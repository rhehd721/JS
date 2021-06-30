# JS

## 문법
```js
var 갑을 = "병정";
var Früh = "foobar"; // Früh: 독일어로 "이른"

myVariable === 4;   // 동등
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
- 함수 호스팅
```js
/* 함수 선언 */

foo(); // "bar"

function foo() {
  console.log('bar');
}


/* 함수 표현식 */

baz(); // TypeError: baz is not a function

var baz = function() {
  console.log('bar2');
};
```
## 자료형 변환
```js
var answer = 42;
answer = "Thanks for all the fish...";

x = "The answer is " + 42 // "The answer is 42"
y = 42 + " is the answer" // "42 is the answer"

// + 연산자의 특성
"37" - 7 // 30
"37" + 7 // 377

"1.1" + "1.1" = "1.11.1"
(+"1.1") + (+"1.1") = 2.2
```
## 리터럴
- 배열 리터럴
```js
var coffees = ["French Roast", "Colombian", "Kona"];
```
- 불리언 리터럴
```js
var x = new Boolean(false);
if (x) {
  // 이 코드는 실행됨
}

var x = false;
if (x) {
  // 이 코드는 실행되지 않음
}
```
- 객체 리터럴
```js
var car = { manyCars: {a: "Saab", "b": "Jeep"}, 7: "Mazda" };

console.log(car.manyCars.b); // Jeep
console.log(car[7]); // Mazda

var foo = {a: "alpha", 2: "two"};
console.log(foo.a);    // alpha
console.log(foo[2]);   // two
//console.log(foo.2);  // Error: missing ) after argument list
//console.log(foo[a]); // Error: a is not defined
console.log(foo["a"]); // alpha
console.log(foo["2"]); // two
```
- 문자열 리터럴
```js

```
