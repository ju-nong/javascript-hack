## structuredClone

```javascript
// 깊은 복사된 객체를 반환
// 배열이나 객체의 요소가 참조 타입일 때 사용

const parentList = [{ name: "이준용" }, { name: "아리" }];

/* ========================================================= */
// 얕은 복사
const childList = [...parentList];
childList[1].name = "아리2";

console.log(parentList[1].name); // "아리2"
/* ========================================================= */
// 깊은 복사
// const childList = JSON.parse(JSON.stringify(parentList)); 권장되지 않음
const childList = structuredClone(parentList);
childList[0].name = "아리2";

consle.log(parentList[0].name); // "아리2"
```
