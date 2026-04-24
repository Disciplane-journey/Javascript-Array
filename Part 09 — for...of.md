# Part 09 — for...of

## Basic Usage

Loops through an array and gives you values directly.

```js
let arr = [10, 20, 30]

for (let value of arr) {
  console.log(value) // 10, 20, 30
}
```

---

## Real World Example

```js
let students = ["Ali", "Sara", "Ahmed"]

for (let name of students) {
  console.log(`Hello ${name}!`)
}

// Hello Ali!
// Hello Sara!
// Hello Ahmed!
```

---

## Comparison — All 3 Loops

```js
let arr = [10, 20, 30]

// forEach
arr.forEach((value) => console.log(value)) // 10, 20, 30

// for...in
for (let key in arr) { console.log(key) }   // "0", "1", "2"

// for...of
for (let value of arr) { console.log(value) } // 10, 20, 30
```

---

## Quick Reference

| Loop | Best for | Gives you |
|------|----------|-----------|
| forEach() | Arrays | value, index, array |
| for...in | Objects | Keys |
| for...of | Arrays | Values directly |

---

## Rule

- Need index? → forEach()
- Looping object? → for...in
- Just need values? → for...of

> JavaScript Array Series
