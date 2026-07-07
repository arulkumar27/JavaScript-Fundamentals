# JavaScript Template Literals

## Introduction

Template literals were introduced in ES6 and use backticks (` `) instead of quotes.

They make it easy to create dynamic strings using variables and expressions.

---

## Basic Syntax

```javascript
const name = "Arul";

console.log(`Hello ${name}`);
```

Output

```
Hello Arul
```

---

## Multiple Variables

```javascript
const name = "Arul";
const age = 22;

console.log(`My name is ${name} and I am ${age} years old.`);
```

---

## Expressions

```javascript
const a = 10;
const b = 20;

console.log(`Sum = ${a + b}`);
```

Output

```
Sum = 30
```

---

## Multi-line Strings

```javascript
const message = `
Welcome
to
JavaScript
`;

console.log(message);
```

---

## Function Calls

```javascript
function greet(name) {
    return `Hello ${name}`;
}

console.log(greet("Arul"));
```

---

## Real-world Example

```javascript
const customer = "Arul";
const amount = 2499;

console.log(
`Dear ${customer},

Your payment of ₹${amount} was successful.

Thank you for shopping with us.`
);
```

---

## Advantages

- Cleaner syntax
- Supports multi-line strings
- Easy variable interpolation
- Better readability
- Reduces string concatenation

---

## Best Practices

- Use template literals instead of `+` for concatenation.
- Keep templates readable.
- Use expressions when needed.

---

## Interview Questions

1. What are template literals?
2. Why use backticks instead of quotes?
3. What is string interpolation?
4. Can template literals span multiple lines?
5. What are the advantages of template literals?

---

## Summary

Template literals provide a modern, readable, and efficient way to create dynamic strings in JavaScript. They are widely used in modern web development.
