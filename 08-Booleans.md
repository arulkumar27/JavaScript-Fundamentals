# JavaScript Booleans

## Introduction

A Boolean represents one of two values:

- true
- false

Booleans are commonly used in conditions and decision-making.

---

## Creating Booleans

```javascript
let isLoggedIn = true;
let isAdmin = false;
```

---

## Comparison

```javascript
console.log(10 > 5);
console.log(20 < 5);
console.log(10 === 10);
```

---

## Logical Operators

AND

```javascript
true && true
```

OR

```javascript
true || false
```

NOT

```javascript
!true
```

---

## Real-world Example

```javascript
let age = 21;

let canVote = age >= 18;

console.log(canVote);
```

---

## Truthy Values

```javascript
1
"Hello"
[]
{}
```

---

## Falsy Values

```javascript
0
""
null
undefined
NaN
false
```

---

## Best Practices

- Write meaningful boolean variable names like `isLoggedIn` or `hasPermission`.
- Avoid comparing booleans unnecessarily (e.g., use `if (isAdmin)` instead of `if (isAdmin === true)`).

---

## Interview Questions

1. What is a Boolean?
2. What are truthy and falsy values?
3. Explain logical operators.
4. Difference between `==` and `===`?
5. Where are Booleans commonly used?

---

## Summary

Booleans control the flow of applications by evaluating conditions and making decisions.
