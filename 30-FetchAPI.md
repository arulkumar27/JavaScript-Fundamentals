# JavaScript Fetch API

## Introduction

The Fetch API is a modern JavaScript interface used to send HTTP requests and receive responses from servers. It is commonly used to communicate with REST APIs.

---

## Why Use Fetch API?

The Fetch API allows developers to:

- Retrieve data from a server
- Send data to a server
- Update existing records
- Delete records
- Build dynamic web applications

---

## Basic GET Request

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

## Using Async/Await

```javascript
async function getPosts() {

    try {

        const response = await fetch(
            "https://jsonplaceholder.typicode.com/posts"
        );

        const posts = await response.json();

        console.log(posts);

    } catch(error) {

        console.log(error);

    }

}

getPosts();
```

---

## POST Request

```javascript
fetch("https://jsonplaceholder.typicode.com/posts", {

    method: "POST",

    headers: {

        "Content-Type": "application/json"

    },

    body: JSON.stringify({

        title: "JavaScript",
        body: "Learning Fetch API",
        userId: 1

    })

})
.then(response => response.json())
.then(data => console.log(data));
```

---

## HTTP Methods

| Method | Purpose |
|---------|----------|
| GET | Retrieve data |
| POST | Create data |
| PUT | Update existing data |
| PATCH | Update partial data |
| DELETE | Delete data |

---

## Response Status

```javascript
fetch(url)
.then(response => {

    if(!response.ok){

        throw new Error("Network Error");

    }

    return response.json();

})
.catch(console.log);
```

---

## Real-world Example

```javascript
async function loadUsers() {

    const response = await fetch(
        "https://jsonplaceholder.typicode.com/users"
    );

    const users = await response.json();

    users.forEach(user => {

        console.log(user.name);

    });

}

loadUsers();
```

---

## Best Practices

- Always check `response.ok`.
- Use try...catch with Async/Await.
- Handle network failures gracefully.
- Validate server responses before using them.

---

## Interview Questions

1. What is the Fetch API?
2. Difference between Fetch API and XMLHttpRequest?
3. How do you send a POST request?
4. What is response.json()?
5. Why should response.ok be checked?

---

## Summary

The Fetch API is the standard way to perform HTTP requests in modern JavaScript. It is widely used for consuming REST APIs and building interactive web applications.
