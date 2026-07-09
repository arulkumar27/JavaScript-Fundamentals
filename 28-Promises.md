# JavaScript Promises

## Introduction

A Promise is an object that represents the eventual completion or failure of an asynchronous operation. It helps write cleaner asynchronous code and avoids callback hell.

---

## Promise States

A Promise has three possible states:

- **Pending** – Initial state, operation is in progress.
- **Fulfilled** – Operation completed successfully.
- **Rejected** – Operation failed.

```
Pending
   │
   ├──► Fulfilled
   │
   └──► Rejected
```

---

## Creating a Promise

```javascript
const promise = new Promise((resolve, reject) => {

    let success = true;

    if (success) {
        resolve("Data fetched successfully.");
    } else {
        reject("Failed to fetch data.");
    }

});
```

---

## Consuming a Promise

```javascript
promise
    .then((result) => {
        console.log(result);
    })
    .catch((error) => {
        console.log(error);
    });
```

---

## Promise Example

```javascript
function loginUser() {

    return new Promise((resolve) => {

        setTimeout(() => {
            resolve("Login Successful");
        }, 2000);

    });

}

loginUser()
    .then((message) => {
        console.log(message);
    });
```

---

## Promise Chaining

```javascript
function getUser() {
    return Promise.resolve("User");
}

function getOrders() {
    return Promise.resolve("Orders");
}

getUser()
    .then((user) => {
        console.log(user);
        return getOrders();
    })
    .then((orders) => {
        console.log(orders);
    })
    .catch((error) => {
        console.log(error);
    });
```

---

## Promise Methods

### Promise.resolve()

```javascript
Promise.resolve("Success")
    .then(console.log);
```

### Promise.reject()

```javascript
Promise.reject("Error")
    .catch(console.log);
```

### Promise.all()

Runs multiple promises in parallel.

```javascript
Promise.all([
    Promise.resolve("HTML"),
    Promise.resolve("CSS"),
    Promise.resolve("JavaScript")
]).then(console.log);
```

---

## Real-world Example

Fetching products from an API:

```javascript
fetch("https://jsonplaceholder.typicode.com/posts")
    .then(response => response.json())
    .then(data => {
        console.log(data);
    })
    .catch(error => {
        console.log(error);
    });
```

---

## Best Practices

- Always handle errors using `.catch()`.
- Use Promise chaining instead of nested callbacks.
- Use `Promise.all()` when multiple tasks can run together.
- Keep Promise logic simple.

---

## Interview Questions

1. What is a Promise?
2. What are the three Promise states?
3. Difference between resolve() and reject()?
4. What is Promise.all()?
5. How do Promises solve callback hell?

---

## Summary

Promises make asynchronous JavaScript easier to read, maintain, and debug by providing a structured way to handle asynchronous operations.
