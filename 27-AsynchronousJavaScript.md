# Asynchronous JavaScript

## Introduction

JavaScript is a single-threaded language, meaning it executes one task at a time. However, some operations like fetching data from a server or reading a file take time.

Instead of stopping the entire program, JavaScript performs these tasks asynchronously.

---

# Synchronous vs Asynchronous

## Synchronous

Tasks execute one after another.

```javascript
console.log("Task 1");
console.log("Task 2");
console.log("Task 3");
```

Output

```
Task 1
Task 2
Task 3
```

---

## Asynchronous

Some tasks run in the background without blocking the rest of the program.

```javascript
console.log("Start");

setTimeout(() => {
    console.log("Task Completed");
}, 2000);

console.log("End");
```

Output

```
Start
End
Task Completed
```

---

# Why Asynchronous Programming?

Without asynchronous programming:

- Websites would freeze while waiting for data.
- Users would experience poor performance.

With asynchronous programming:

- Better user experience
- Faster applications
- Non-blocking operations

---

# Common Asynchronous Operations

- API Requests
- Database Queries
- File Uploads
- Timers
- User Authentication
- Reading Files

---

# setTimeout()

Executes a function after a specified delay.

```javascript
setTimeout(() => {
    console.log("Hello after 3 seconds");
}, 3000);
```

---

# setInterval()

Executes a function repeatedly after a fixed interval.

```javascript
setInterval(() => {
    console.log("Running...");
}, 1000);
```

---

# Callback Function

A callback is a function passed as an argument to another function.

```javascript
function greet(name, callback) {
    console.log("Hello " + name);
    callback();
}

function goodbye() {
    console.log("Goodbye!");
}

greet("Arul", goodbye);
```

---

# Callback Hell

Nested callbacks make code difficult to read.

```javascript
login(function () {
    getUser(function () {
        getOrders(function () {
            console.log("Done");
        });
    });
});
```

This problem is solved using Promises and Async/Await.

---

# Real-world Example

```javascript
console.log("Loading products...");

setTimeout(() => {
    console.log("Products Loaded");
}, 2000);
```

---

# Best Practices

- Avoid deeply nested callbacks.
- Use Promises or Async/Await for cleaner code.
- Handle asynchronous errors properly.
- Keep asynchronous logic readable.

---

# Interview Questions

1. What is asynchronous programming?
2. Difference between synchronous and asynchronous execution?
3. What is a callback function?
4. What is callback hell?
5. Why do we need asynchronous programming?

---

# Summary

Asynchronous JavaScript allows applications to perform time-consuming operations without blocking the main thread, resulting in faster and more responsive web applications.
