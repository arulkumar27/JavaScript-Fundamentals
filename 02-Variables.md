# Variables in JavaScript

## What is a Variable?

A variable is a named storage location used to store data that can be accessed or modified later in the program.

---

## Variable Keywords

JavaScript provides three ways to declare variables:

- var
- let
- const

---

## Using let

```javascript
let name = "Arul";
console.log(name);
```

The value can be changed later.

```javascript
let age = 22;
age = 23;
```

---

## Using const

```javascript
const country = "India";
```

A constant cannot be reassigned.

---

## Using var

```javascript
var city = "Chennai";
```

Older syntax and generally avoided in modern JavaScript.

---

## Naming Rules

✅ Valid

```javascript
userName
first_name
student1
```

❌ Invalid

```javascript
1name
user-name
var
```

---

## Best Practices

- Prefer const whenever possible.
- Use let when values change.
- Avoid var in new projects.

---

## Real-world Example

```javascript
const website = "Amazon";
let cartItems = 3;

cartItems++;

console.log(cartItems);
```

---

## Summary

Variables allow developers to store and manage data efficiently throughout a program.
