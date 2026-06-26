# JavaScript Data Types

## Introduction

Data types define the kind of value stored in a variable.

---

## Primitive Data Types

### String

```javascript
let name = "Arul";
```

---

### Number

```javascript
let age = 22;
```

Supports integers and decimals.

---

### Boolean

```javascript
let isLoggedIn = true;
```

---

### Undefined

```javascript
let address;
```

---

### Null

```javascript
let data = null;
```

---

### Symbol

Used for creating unique identifiers.

```javascript
const id = Symbol("id");
```

---

### BigInt

Stores very large integers.

```javascript
const number = 123456789012345678901234567890n;
```

---

## Non-Primitive Data Types

### Object

```javascript
const student = {
    name: "Arul",
    age: 22
};
```

---

### Array

```javascript
const colors = ["Red","Blue","Green"];
```

---

### Function

```javascript
function greet(){
    console.log("Hello");
}
```

---

## Real-world Example

A shopping website stores:

- Product Name → String
- Price → Number
- Available → Boolean
- Product Details → Object
- Reviews → Array

---

## Summary

Understanding data types helps developers write accurate and efficient JavaScript programs.
