# JavaScript Async/Await

## Introduction

`async` and `await` are modern JavaScript features introduced in ES2017. They provide a cleaner and more readable way to work with Promises.

---

## Why Async/Await?

Without Async/Await:

```javascript
fetchData()
    .then(data => processData(data))
    .then(result => console.log(result))
    .catch(error => console.log(error));
```

With Async/Await:

```javascript
async function loadData() {

    try {

        const data = await fetchData();

        console.log(data);

    } catch(error) {

        console.log(error);

    }

}
```

Much easier to understand.

---

## async Function

```javascript
async function greet() {
    return "Hello";
}

greet().then(console.log);
```

Output

```
Hello
```

---

## await Keyword

```javascript
function delay() {

    return new Promise(resolve => {

        setTimeout(() => {

            resolve("Completed");

        }, 2000);

    });

}

async function run() {

    const result = await delay();

    console.log(result);

}

run();
```

---

## Error Handling

```javascript
async function getData() {

    try {

        const response = await fetch("https://jsonplaceholder.typicode.com/users");

        const data = await response.json();

        console.log(data);

    }

    catch(error) {

        console.log(error);

    }

}
```

---

## Real-world Example

```javascript
async function getProducts() {

    const response = await fetch("https://jsonplaceholder.typicode.com/posts");

    const products = await response.json();

    console.log(products);

}

getProducts();
```

---

## Advantages

- Cleaner syntax
- Easier debugging
- Better readability
- Eliminates callback hell
- Simplifies Promise handling

---

## Best Practices

- Always use try...catch.
- Await only Promises.
- Avoid unnecessary await statements.
- Use Promise.all() for parallel operations.

---

## Interview Questions

1. What is async?
2. What does await do?
3. Can await be used outside an async function?
4. Difference between Promises and Async/Await?
5. Why use try...catch?

---

## Summary

Async/Await is the preferred approach for handling asynchronous code because it makes JavaScript applications cleaner, easier to read, and easier to maintain.
