# Part 08 — for...in

## What is for...in?

for...in loops through the **keys** of an object — not the values.

```js
let obj = {
  name: "Ali",
  age: 20,
  city: "Karachi"
}

for (let key in obj) {
  console.log(key)       // name, age, city
  console.log(obj[key])  // Ali, 20, Karachi
}
```

---

## Using for...in on arrays

for...in works on arrays — but gives you string indexes as keys.

```js
let arr = [10, 20, 30]

for (let key in arr) {
  console.log(key)      // "0", "1", "2" — string keys
  console.log(arr[key]) // 10, 20, 30
}
```

This can cause unexpected behavior — avoid using for...in on arrays.

---

## Correct Use Case

```js
let user = { name: "Ali", age: 20 }

for (let key in user) {
  console.log(`${key}: ${user[key]}`)
}

// name: Ali
// age: 20
```

---

## Rule

| | for...in |
|---|---|
| Best for | Objects |
| Gives you | Keys |
| Use on arrays | Never |

> JavaScript Array Series
