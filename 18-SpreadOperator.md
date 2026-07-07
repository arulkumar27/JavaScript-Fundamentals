# JavaScript Spread Operator

## Introduction

The Spread Operator (`...`) was introduced in ES6. It expands elements of an array or properties of an object into individual elements.

It is commonly used for copying arrays, merging arrays, copying objects, and passing arguments to functions.

---

## Syntax

```javascript
...
```

---

## Copying an Array

```javascript
const numbers = [1, 2, 3];

const copiedNumbers = [...numbers];

console.log(copiedNumbers);
```

Output

```
[1, 2, 3]
```

---

## Merging Arrays

```javascript
const frontend = ["HTML", "CSS"];
const backend = ["Node.js", "Express"];

const fullStack = [...frontend, ...backend];

console.log(fullStack);
```

Output

```
["HTML", "CSS", "Node.js", "Express"]
```

---

## Copying an Object

```javascript
const student = {
    name: "Arul",
    age: 22
};

const copyStudent = {
    ...student
};

console.log(copyStudent);
```

---

## Merging Objects

```javascript
const personal = {
    name: "Arul"
};

const professional = {
    role: "Developer"
};

const profile = {
    ...personal,
    ...professional
};

console.log(profile);
```

---

## Passing Function Arguments

```javascript
const numbers = [10, 20, 30];

console.log(Math.max(...numbers));
```

Output

```
30
```

---

## Real-world Example

```javascript
const cart1 = ["Laptop", "Mouse"];
const cart2 = ["Keyboard", "Monitor"];

const finalCart = [...cart1, ...cart2];

console.log(finalCart);
```

---

## Best Practices

- Use spread for copying arrays and objects.
- Avoid modifying the original data.
- Useful in React state management.
- Makes code cleaner than manual copying.

---

## Interview Questions

1. What is the spread operator?
2. Difference between spread and rest operator?
3. How do you merge arrays?
4. How do you copy objects?
5. Why is spread operator useful?

---

## Summary

The spread operator simplifies copying, merging, and expanding arrays and objects, making JavaScript code more concise and readable.
