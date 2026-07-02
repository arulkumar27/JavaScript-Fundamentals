# JavaScript Arrays

## Introduction

An array stores multiple values in a single variable.

---

## Creating Arrays

```javascript
let fruits = ["Apple", "Orange", "Banana"];
```

---

## Accessing Elements

```javascript
console.log(fruits[0]);
console.log(fruits[1]);
```

---

## Updating Elements

```javascript
fruits[2] = "Mango";
```

---

## Array Length

```javascript
console.log(fruits.length);
```

---

## Adding Elements

```javascript
fruits.push("Grapes");
fruits.unshift("Kiwi");
```

---

## Removing Elements

```javascript
fruits.pop();
fruits.shift();
```

---

## Looping Through Arrays

```javascript
for(let fruit of fruits){
    console.log(fruit);
}
```

---

## Real-world Example

```javascript
let cart = [
    "Laptop",
    "Mouse",
    "Keyboard"
];

console.log(cart);
```

---

## Best Practices

- Store similar data together.
- Use meaningful variable names.
- Prefer array methods instead of manual indexing.

---

## Interview Questions

1. What is an array?
2. Difference between push() and unshift()?
3. Difference between pop() and shift()?
4. How do you access array elements?
5. How do you loop through arrays?

---

## Summary

Arrays are one of the most commonly used data structures in JavaScript for storing collections of data.
