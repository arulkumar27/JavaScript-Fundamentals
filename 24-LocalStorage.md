# JavaScript Local Storage

## Introduction

Local Storage is a Web Storage API that allows websites to store data in the user's browser.

The stored data remains available even after the browser is closed and reopened.

---

# Features

- Stores data as key-value pairs
- Data persists until manually removed
- Storage limit is approximately 5–10 MB
- Accessible only from the same origin

---

# Storing Data

```javascript
localStorage.setItem("username", "Arul");
```

---

# Retrieving Data

```javascript
const username = localStorage.getItem("username");

console.log(username);
```

Output

```
Arul
```

---

# Updating Data

```javascript
localStorage.setItem("username", "Kumar");
```

---

# Removing Data

```javascript
localStorage.removeItem("username");
```

---

# Clearing All Data

```javascript
localStorage.clear();
```

---

# Storing Objects

```javascript
const user = {
    name: "Arul",
    age: 22
};

localStorage.setItem(
    "user",
    JSON.stringify(user)
);
```

---

# Retrieving Objects

```javascript
const user = JSON.parse(
    localStorage.getItem("user")
);

console.log(user.name);
```

---

# Real-world Example

Save the selected website theme.

```javascript
localStorage.setItem("theme", "dark");
```

When the user visits again, the website can automatically load the saved theme.

---

# Best Practices

- Store only necessary data.
- Convert objects using JSON.stringify().
- Use JSON.parse() when retrieving objects.
- Avoid storing sensitive information like passwords or tokens.

---

# Interview Questions

1. What is Local Storage?
2. Does Local Storage expire?
3. Difference between Local Storage and Cookies?
4. Why use JSON.stringify()?
5. Can Local Storage store objects directly?

---

# Summary

Local Storage is useful for storing user preferences, themes, shopping carts, and other persistent browser data.
