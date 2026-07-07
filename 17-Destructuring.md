# JavaScript Destructuring

## Introduction

Destructuring is an ES6 feature that allows you to extract values from arrays and objects into separate variables.

It makes code cleaner, shorter, and easier to read.

---

## Why Use Destructuring?

Benefits include:

- Less code
- Improved readability
- Easy extraction of values
- Commonly used in React and Node.js

---

## Array Destructuring

```javascript
const colors = ["Red", "Blue", "Green"];

const [first, second, third] = colors;

console.log(first);
console.log(second);
console.log(third);
```

Output

```
Red
Blue
Green
```

---

## Skipping Values

```javascript
const numbers = [10,20,30,40];

const [a,,c] = numbers;

console.log(a);
console.log(c);
```

Output

```
10
30
```

---

## Object Destructuring

```javascript
const student = {
    name: "Arul",
    age: 22,
    city: "Salem"
};

const { name, age } = student;

console.log(name);
console.log(age);
```

Output

```
Arul
22
```

---

## Renaming Variables

```javascript
const { name: studentName } = student;

console.log(studentName);
```

---

## Default Values

```javascript
const user = {
    username: "Arul"
};

const { username, role = "Student" } = user;

console.log(role);
```

Output

```
Student
```

---

## Nested Destructuring

```javascript
const employee = {
    id: 101,
    address: {
        city: "Salem",
        state: "Tamil Nadu"
    }
};

const {
    address: { city }
} = employee;

console.log(city);
```

---

## Real-world Example

```javascript
const product = {
    name: "Laptop",
    price: 55000,
    brand: "Dell"
};

const { name, price } = product;

console.log(`${name} costs ₹${price}`);
```

---

## Best Practices

- Use destructuring for cleaner code.
- Rename variables when necessary.
- Use default values to avoid undefined.
- Keep nested destructuring readable.

---

## Interview Questions

1. What is destructuring?
2. Difference between array and object destructuring?
3. How do you rename variables while destructuring?
4. How do default values work?
5. What is nested destructuring?

---

## Summary

Destructuring simplifies working with arrays and objects, making JavaScript code more concise, readable, and maintainable.
