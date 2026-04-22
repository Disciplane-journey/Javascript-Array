<img width="1017" height="678" alt="code_20260423_034141_via_10015_io" src="https://github.com/user-attachments/assets/488e27bd-2ff1-4133-819d-7353456cad98" />
# Part 01 — Arrays Basics

## What is an Array?

An array is a data structure that stores multiple values in a single variable.

```js
let arr = [1, 2, 3]
```

---

## Arrays are Mutable

You can go to any index and change the value directly.

```js
let arr = [1, 2, 3]
arr[0] = 111

console.log(arr) // [111, 2, 3] ✅
```

---

## Strings are NOT Mutable

```js
let str = "hello"
str[0] = "H"

console.log(str) // "hello" ❌
```

No error. No warning. JavaScript silently ignores it.

---

## typeof Array returns "object"

```js
typeof [1, 2, 3] // "object"
```

An array in JavaScript is actually a special object where keys are 0, 1, 2...

So never use typeof to check if something is an array. Use this instead:

```js
Array.isArray([1, 2, 3]) // true ✅
```

---

> JavaScript Array Series
