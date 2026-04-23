# Part 03 — push(), pop(), shift(), unshift()

## push() — Add at the end

```js
let arr = [1, 2, 3]

arr.push(4)
console.log(arr) // [1, 2, 3, 4] ✅
```

---

## pop() — Remove from the end

```js
let arr = [1, 2, 3]

arr.pop()
console.log(arr) // [1, 2] ✅
```

---

## unshift() — Add at the beginning

```js
let arr = [1, 2, 3]

arr.unshift(0)
console.log(arr) // [0, 1, 2, 3] ✅
```

---

## shift() — Remove from the beginning

```js
let arr = [1, 2, 3]

arr.shift()
console.log(arr) // [2, 3] ✅
```

---

## Quick Reference

| Method | Action | Position |
|--------|--------|----------|
| push() | Add | End |
| pop() | Remove | End |
| unshift() | Add | Beginning |
| shift() | Remove | Beginning |

---

## Important

All 4 methods modify the original array directly.

> JavaScript Array Series
