## GCD

```javascript
// 최대공약수 구하기 (유클리드 호제법)

let [a, b] = [50, 15];

while (b) {
  [a, b] = [b, a % b];
}

console.log(a); // 5
```
