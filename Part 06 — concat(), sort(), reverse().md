# Part 06 — concat(), sort(), reverse()

## concat() — Join arrays

Joins two or more arrays and returns a new array.
Original array is never modified.

```js
let arr1 = [1, 2, 3]
let arr2 = [4, 5, 6]

let result = arr1.concat(arr2)
console.log(result) // [1, 2, 3, 4, 5, 6] ✅
console.log(arr1)   // [1, 2, 3] — no change ✅
```

---

## sort() — Sort the array

Sorts the array directly — modifies the original.

```js
let arr = [3, 1, 4, 2]

arr.sort()
console.log(arr) // [1, 2, 3, 4] ✅
```

### Important — Sorting numbers correctly

By default sort() sorts as strings — always use a compare function for numbers:

```js
let arr = [10, 9, 2, 100]

arr.sort((a, b) => a - b)
console.log(arr) // [2, 9, 10, 100] ✅
```

---

## reverse() — Reverse the array

Reverses the array directly — modifies the original.

```js
let arr = [1, 2, 3, 4]

arr.reverse()
console.log(arr) // [4, 3, 2, 1] ✅
```

---

## Quick Reference

| Method | Changes Original | Returns |
|--------|-----------------|---------|
| concat() | ❌ Never | New array |
| sort() | ✅ Always | Sorted array |
| reverse() | ✅ Always | Reversed array |

> JavaScript Array Series
