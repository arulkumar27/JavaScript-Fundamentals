# JavaScript Array Methods

## Introduction

JavaScript provides many built-in methods to manipulate arrays efficiently.

---

## push()

Adds an element to the end.

```javascript
let numbers = [1,2,3];

numbers.push(4);
```

---

## pop()

Removes the last element.

```javascript
numbers.pop();
```

---

## shift()

Removes the first element.

```javascript
numbers.shift();
```

---

## unshift()

Adds an element to the beginning.

```javascript
numbers.unshift(0);
```

---

## includes()

Checks whether an element exists.

```javascript
console.log(numbers.includes(2));
```

---

## indexOf()

Returns the position.

```javascript
console.log(numbers.indexOf(3));
```

---

## join()

Converts an array into a string.

```javascript
console.log(numbers.join("-"));
```

---

## reverse()

```javascript
numbers.reverse();
```

---

## sort()

```javascript
numbers.sort();
```

---

## Real-world Example

```javascript
let shoppingCart = [
    "Laptop",
    "Mouse",
    "Keyboard"
];

shoppingCart.push("Headphones");

console.log(shoppingCart);
```

---

## Best Practices

- Use built-in methods instead of manual loops when appropriate.
- Understand which methods modify the original array.
- Use descriptive variable names.

---

## Interview Questions

1. Difference between push() and pop()?
2. What does includes() return?
3. Difference between shift() and unshift()?
4. How does sort() work?
5. What does join() do?

---

## Summary

Array methods simplify common tasks like adding, removing, searching, sorting, and transforming data, making JavaScript code cleaner and more efficient.
