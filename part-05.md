# Part 05 — slice() vs splice()

## slice() — Copy without modifying

Extracts elements and returns them as a new array.
Original array is never touched.

```js
let arr = [1, 2, 3, 4, 5]

let result = arr.slice(1, 3)
console.log(result) // [2, 3] ✅
console.log(arr)    // [1, 2, 3, 4, 5] — no change ✅
```

slice(startIndex, endIndex) — endIndex is not included.

---

## splice() — Remove from original

Removes elements directly from the original array.

```js
let arr = [1, 2, 3, 4, 5]

arr.splice(1, 3)
console.log(arr) // [1, 5] ✅
```

splice(startIndex, deleteCount)

---

## Key Difference

| | slice() | splice() |
|---|---|---|
| Changes original | ❌ Never | ✅ Always |
| Returns | Copied elements | Removed elements |
| Use case | Read only | Remove or Add |

---

## Easy Way to Remember

- slice → like slicing bread — you get a piece but the loaf is still there 🍞
- splice → like surgery — you cut something out and it's gone 🔪

> JavaScript Array Series
