# Part 11 — Array.from()

## What is Array.from()?

Converts array-like or iterable objects into a real array.

---

## String to array

```js
Array.from("hello")
// ["h", "e", "l", "l", "o"] ✅
```

---

## Remove duplicates with Set

```js
let nums = [1, 2, 2, 3, 3, 4]

Array.from(new Set(nums))
// [1, 2, 3, 4] ✅
```

Set removes duplicates — Array.from() converts it back to an array.

---

## NodeList to array

```js
let divs = document.querySelectorAll("div")

let divsArray = Array.from(divs)

divsArray.map(div => div.innerText)
divsArray.filter(div => div.classList.contains("active"))
```

querySelectorAll returns a NodeList — not a real array.
Array.from() converts it so you can use map(), filter(), reduce() on it.

---

## With a map function

```js
Array.from([1, 2, 3], x => x * 2)
// [2, 4, 6] ✅
```

Create and transform in one step.

---

## Quick Reference

| Input | Output |
|-------|--------|
| String | Array of characters |
| Set | Array without duplicates |
| NodeList | Real array |
| Array-like object | Real array |

> JavaScript Array Series
