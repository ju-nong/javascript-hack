## DFS

```javascript
// 깊이 우선 탐색

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

function DFS(node, arr) {
    arr.push(node);

    const children = graph[node];
    for (let i = 0; i < children.length; i++) {
        DFS(children[i], arr);
    }

    return arr;
}

console.log(DFS("A", [])); // ["A", "B", "D", "E", "F", "C", "G", "H", "I", "J"]
```
