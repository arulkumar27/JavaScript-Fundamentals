# JavaScript Functions

## Introduction

A function is a reusable block of code designed to perform a specific task. Instead of writing the same code multiple times, you can define it once and call it whenever needed.

---

## Why Use Functions?

Functions help you:

- Reuse code
- Improve readability
- Reduce duplication
- Organize programs into smaller modules
- Make debugging easier

---

## Function Declaration

```javascript
function greet() {
    console.log("Welcome to JavaScript!");
}

greet();
```

---

## Function with Parameters

```javascript
function greet(name) {
    console.log("Hello " + name);
}

greet("Arul");
```

---

## Returning Values

```javascript
function add(a, b) {
    return a + b;
}

let result = add(10, 20);
console.log(result);
```

---

## Function Expression

```javascript
const multiply = function(a, b) {
    return a * b;
};

console.log(multiply(5, 4));
```

---

## Real-world Example

```javascript
function calculateBill(price, quantity) {
    return price * quantity;
}

console.log(calculateBill(500, 3));
```

---

## Best Practices

- Keep functions short.
- Give meaningful names.
- Return values instead of printing whenever possible.
- Avoid global variables.

---

## Interview Questions

1. What is a function?
2. Why use functions?
3. Difference between parameters and arguments?
4. What is a return statement?
5. What is a function expression?

---

## Summary

Functions make JavaScript applications modular, reusable, and easier to maintain.
