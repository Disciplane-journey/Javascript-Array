# Part 04 — delete vs splice()

## delete

Removes the value but leaves the slot as undefined.

```js
let arr = [1, 2, 3, 4, 5]

delete arr[1]
console.log(arr)        // [1, undefined, 3, 4, 5] ❌
console.log(arr.length) // 5 — length did not change
```

---

## splice() — Remove elements

Removes elements cleanly — no holes, no undefined.

```js
let arr = [1, 2, 3, 4, 5]

arr.splice(1, 3)
console.log(arr)        // [1, 5] ✅
console.log(arr.length) // 2 — length updated correctly
```

splice(startIndex, deleteCount)

| Parameter | Meaning |
|-----------|---------|
| startIndex | Where to start |
| deleteCount | How many to remove |

---

## splice() — Add elements back

```js
let arr = [1, 5]

arr.splice(1, 0, 2, 3, 4)
console.log(arr) // [1, 2, 3, 4, 5] ✅
```

splice(1, 0, 2, 3, 4) — start at index 1, remove 0, add 2, 3, 4.

---

## Key Difference

| | delete | splice() |
|---|---|---|
| Removes value | ✅ | ✅ |
| Removes slot | ❌ | ✅ |
| Updates length | ❌ | ✅ |
| Leaves undefined | ✅ | ❌ |

---

## Rule

Never use delete on arrays — always use splice()

> JavaScript Array Series
