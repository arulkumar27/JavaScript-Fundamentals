# JavaScript Strings

## Introduction

A string is a sequence of characters used to represent text. Strings are enclosed in single quotes (' '), double quotes (" "), or backticks (` `).

---

## Creating Strings

```javascript
let firstName = "Arul";
let lastName = 'Kumar';
let city = `Salem`;
```

---

## String Concatenation

```javascript
let fullName = firstName + " " + lastName;

console.log(fullName);
```

Output

```
Arul Kumar
```

---

## Template Literals

Template literals make it easier to insert variables into strings.

```javascript
let name = "Arul";
let age = 22;

console.log(`My name is ${name} and I am ${age} years old.`);
```

---

## Common String Methods

```javascript
let text = "JavaScript";

console.log(text.length);
console.log(text.toUpperCase());
console.log(text.toLowerCase());
console.log(text.includes("Script"));
console.log(text.startsWith("Java"));
console.log(text.endsWith("Script"));
console.log(text.slice(0,4));
console.log(text.replace("Java","Type"));
```

---

## Real-world Example

Displaying a welcome message after login:

```javascript
let username = "Arul";

console.log(`Welcome back, ${username}!`);
```

---

## Best Practices

- Use template literals for readability.
- Avoid unnecessary string concatenation.
- Use meaningful variable names.

---

## Interview Questions

1. What is a string?
2. Difference between concatenation and template literals?
3. What does `slice()` do?
4. Explain `replace()`.
5. What is `includes()`?

---

## Summary

Strings are essential for handling text such as usernames, messages, emails, and URLs in JavaScript applications.
