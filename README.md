# javascript-hack

###### 자바스크립트의 잡기술을 적는 곳

###### Programmer 풀다가 배운 거 기록할거임

<hr />

### +(string)

```javascript
// 문자를 숫자로 바꿔줌

const string = "100";
const number = +string; // 100
```

<br/>

### ~~(number)

```javascript
// 소수점을 없애줌, Math.trunc와 기능은 같음

const a = 100.1234;
const b = ~~a; // 100
```

<br/>

### [...new Set(string)]

```javascript
// 문자열에서 중복을 제거하는 문제였음

const word = "Hello World haha ha";
const result = [...new Set(word)].join(""); // "Helo Wrdha";
```
