# JavaScript Numbers

## Introduction

The Number data type represents both integers and floating-point values.

---

## Creating Numbers

```javascript
let age = 22;
let salary = 55000.75;
```

---

## Arithmetic Operations

```javascript
let a = 20;
let b = 5;

console.log(a + b);
console.log(a - b);
console.log(a * b);
console.log(a / b);
console.log(a % b);
```

---

## Number Methods

```javascript
let num = 123.456;

console.log(num.toFixed(2));
console.log(num.toPrecision(4));
```

---

## Math Object

```javascript
console.log(Math.round(4.6));
console.log(Math.floor(4.9));
console.log(Math.ceil(4.1));
console.log(Math.max(10,20,30));
console.log(Math.min(10,20,30));
console.log(Math.random());
```

---

## Real-world Example

Calculating product price:

```javascript
let price = 799;
let quantity = 2;

let total = price * quantity;

console.log(total);
```

---

## Best Practices

- Validate numeric input.
- Use `Number()` for conversion.
- Avoid floating-point precision issues in financial calculations.

---

## Interview Questions

1. Difference between integer and float?
2. Explain `Math.random()`.
3. What is `toFixed()`?
4. Difference between `Math.floor()` and `Math.ceil()`?
5. What does `%` operator do?

---

## Summary

Numbers are used for calculations such as pricing, salaries, statistics, and business logic.
