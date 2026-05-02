# Part 02 — toString() and join()
<img width="974" height="678" alt="code_20260423_042623_via_10015_io" src="https://github.com/user-attachments/assets/a9644d77-bdd9-4987-ac4a-f34975e00405" />


## toString()

Converts an array into a string — always separated by a comma.

```js
let arr = [1, 2, 3]

arr.toString() // "1,2,3"
```

---

## join()

Converts an array into a string — you choose the separator.

```js
let arr = [1, 2, 3]

arr.join(" and ") // "1 and 2 and 3"
arr.join(" - ")   // "1 - 2 - 3"
arr.join("")      // "123"
```

---

## Key Difference

| | toString() | join() |
|---|---|---|
| Separator | Always comma | You choose |
| Control | None | Full |

---

## Original Array Never Changes

Neither method modifies the original array.

```js
let arr = [1, 2, 3]
arr.join(" - ")

console.log(arr) // [1, 2, 3] ✅
```

---

> JavaScript Array Series
