# Part 07 — forEach()

## Basic Usage

Loop through every element in an array.

```js
let arr = [1, 2, 3]

arr.forEach((value) => {
  console.log(value) // 1, 2, 3
})
```

---

## 3 Parameters

forEach() gives you access to 3 things:

```js
arr.forEach((value, index, array) => {
  console.log(value)  // current element
  console.log(index)  // current position
  console.log(array)  // the full array
})
```

Use only what you need.

---

## Real World Example

```js
let students = ["Ali", "Sara", "Ahmed"]

students.forEach((name, index) => {
  console.log(`${index + 1}. ${name}`)
})

// 1. Ali
// 2. Sara
// 3. Ahmed
```

---

## Important

forEach() never returns anything.

```js
let result = arr.forEach((value) => {
  return value * 2
})

console.log(result) // undefined ❌
```

If you need a new array — use map() instead.

---

## Quick Reference

| | forEach() |
|---|---|
| Returns | Nothing |
| Changes original | ❌ Never |
| Use case | Loop through array |

> JavaScript Array Series
