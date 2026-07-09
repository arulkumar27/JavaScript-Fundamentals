# JavaScript Session Storage

## Introduction

Session Storage is a browser storage mechanism that stores data only for the duration of the current browser tab or window.

Once the tab is closed, all stored data is automatically removed.

---

# Features

- Stores key-value pairs
- Data exists only for the current session
- Different tabs have separate storage
- Storage limit is approximately 5 MB

---

# Storing Data

```javascript
sessionStorage.setItem("username", "Arul");
```

---

# Retrieving Data

```javascript
const username = sessionStorage.getItem("username");

console.log(username);
```

---

# Updating Data

```javascript
sessionStorage.setItem("username", "Kumar");
```

---

# Removing Data

```javascript
sessionStorage.removeItem("username");
```

---

# Clearing Session Storage

```javascript
sessionStorage.clear();
```

---

# Storing Objects

```javascript
const product = {
    id: 101,
    name: "Laptop"
};

sessionStorage.setItem(
    "product",
    JSON.stringify(product)
);
```

---

# Retrieving Objects

```javascript
const product = JSON.parse(
    sessionStorage.getItem("product")
);

console.log(product.name);
```

---

# Local Storage vs Session Storage

| Feature | Local Storage | Session Storage |
|---------|---------------|-----------------|
| Lifetime | Permanent | Until tab closes |
| Shared Across Tabs | Yes | No |
| Capacity | 5–10 MB | ~5 MB |

---

# Real-world Example

Store a multi-step registration form temporarily.

If the user refreshes the page, the data remains available, but it is removed once the browser tab is closed.

---

# Best Practices

- Use Session Storage for temporary data.
- Don't store confidential information.
- Convert objects using JSON methods.
- Clear unused session data.

---

# Interview Questions

1. What is Session Storage?
2. Difference between Local Storage and Session Storage?
3. When should Session Storage be used?
4. Does Session Storage persist after closing the browser?
5. Can Session Storage store objects?

---

# Summary

Session Storage is ideal for temporary browser data such as form inputs, login sessions (non-sensitive), and page-specific information that should disappear when the tab is closed.
