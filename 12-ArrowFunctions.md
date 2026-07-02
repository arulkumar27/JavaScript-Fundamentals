# JavaScript Arrow Functions

## Introduction

Arrow functions were introduced in ES6 to provide a shorter syntax for writing functions.

---

## Basic Syntax

```javascript
const greet = () => {
    console.log("Hello World");
};

greet();
```

---

## Single Parameter

```javascript
const square = number => {
    return number * number;
};

console.log(square(5));
```

---

## Multiple Parameters

```javascript
const add = (a, b) => {
    return a + b;
};

console.log(add(10, 20));
```

---

## Implicit Return

```javascript
const multiply = (a, b) => a * b;

console.log(multiply(4, 5));
```

---

## Returning Objects

```javascript
const student = () => ({
    name: "Arul",
    age: 22
});

console.log(student());
```

---

## Real-world Example

```javascript
const calculateGST = amount => amount * 0.18;

console.log(calculateGST(1000));
```

---

## Advantages

- Less code
- Easier to read
- Perfect for callbacks
- Widely used in React

---

## Interview Questions

1. What is an arrow function?
2. Difference between normal and arrow functions?
3. What is implicit return?
4. Can arrow functions be constructors?
5. How does `this` behave in arrow functions?

---

## Summary

Arrow functions simplify JavaScript code and are commonly used in modern applications.
