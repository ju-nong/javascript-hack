## BFS

```javascript
// 너비 우선 탐색

const graph = {
    A: ["B", "C"],
    B: ["D"],
    C: ["G", "H", "I"],
    D: ["E", "F"],
    E: [],
    F: [],
    G: [],
    H: [],
    I: ["J"],
    J: [],
};

function BFS(root) {
    const arr = [];
    const temp = [root];

    while (temp.length) {
        const node = temp.shift();

        arr.push(node);
        temp.push(...graph[node]);
    }

    return arr;
}

console.log(BFS("A")); // ["A", "B", "C", "D", "G", "H", "I", "E", "F", "J"]
```
