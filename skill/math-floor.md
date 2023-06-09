## ~~(number)

```javascript
// 소수점을 없애줌
// 성능면에서는 Math.trunc보다 나으나, 32비트 범위까지만 지원됨(-2,147,483,648 ~ 2,147,483,647)

const number = -3.14;

let floor_number = ~~number; // -3
floor_number = Math.trunc(number); // -3
floor_number = Math.floor(number); // -4 (Math.floor 같은 경우는 음수일 때 소수점 없애고 -1을 더해버림)
```
