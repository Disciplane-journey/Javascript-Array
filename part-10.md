# Part 10 — map(), filter(), reduce()

## map() — Transform every element

Returns a new array with transformed values.
Original array is never modified.

```js
let arr = [1, 2, 3, 4, 5]

let doubled = arr.map(value => value * 2)
console.log(doubled) // [2, 4, 6, 8, 10] ✅
console.log(arr)     // [1, 2, 3, 4, 5] ✅
```

---

## filter() — Keep only what passes

Returns a new array with only the elements that pass the condition.

```js
let arr = [1, 2, 3, 4, 5]

let bigNumbers = arr.filter(value => value > 3)
console.log(bigNumbers) // [4, 5] ✅
console.log(arr)        // [1, 2, 3, 4, 5] ✅
```

---

## reduce() — Combine into one value

Builds up a single result from every element.

```js
let arr = [1, 2, 3, 4, 5]

// Addition
let total = arr.reduce((sum, value) => sum + value, 0)
console.log(total) // 15 ✅

// Multiplication
let result = arr.reduce((total, value) => total * value, 1)
console.log(result) // 120 ✅
```

reduce(callback, startingValue)

| Parameter | Meaning |
|-----------|---------|
| sum / total | Running result — starts at startingValue |
| value | Current element |

---

## Quick Reference

| Method | Returns | Changes original |
|--------|---------|-----------------|
| map() | New array | ❌ Never |
| filter() | New array | ❌ Never |
| reduce() | Single value | ❌ Never |

> JavaScript Array Series
