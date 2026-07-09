# JavaScript JSON

## Introduction

JSON (JavaScript Object Notation) is a lightweight format used to store and exchange data between a client and a server. It is easy for humans to read and write and easy for machines to parse and generate.

Most REST APIs return data in JSON format.

---

# Why JSON?

JSON is widely used because it is:

- Lightweight
- Easy to read
- Language-independent
- Supported by almost every programming language
- Perfect for API communication

---

# JSON Syntax

```json
{
    "name": "Arul",
    "age": 22,
    "city": "Salem"
}
```

Rules:

- Data is stored as key-value pairs.
- Keys must be enclosed in double quotes.
- Values can be strings, numbers, booleans, arrays, objects, or null.

---

# JavaScript Object

```javascript
const student = {
    name: "Arul",
    age: 22,
    city: "Salem"
};

console.log(student);
```

---

# Convert Object to JSON

Use `JSON.stringify()`.

```javascript
const student = {
    name: "Arul",
    age: 22
};

const jsonData = JSON.stringify(student);

console.log(jsonData);
```

Output

```
{"name":"Arul","age":22}
```

---

# Convert JSON to Object

Use `JSON.parse()`.

```javascript
const json = '{"name":"Arul","age":22}';

const obj = JSON.parse(json);

console.log(obj.name);
```

Output

```
Arul
```

---

# JSON Arrays

```json
[
    {
        "name": "Laptop",
        "price": 55000
    },
    {
        "name": "Mouse",
        "price": 800
    }
]
```

---

# Access JSON Data

```javascript
const user = {
    name: "Arul",
    skills: ["HTML", "CSS", "JavaScript"]
};

console.log(user.skills[2]);
```

Output

```
JavaScript
```

---

# Real-world Example

Receiving API response

```javascript
fetch("https://jsonplaceholder.typicode.com/users/1")
    .then(response => response.json())
    .then(data => {
        console.log(data.name);
    });
```

---

# Best Practices

- Always validate JSON before parsing.
- Use JSON.stringify() when storing objects.
- Use JSON.parse() when retrieving JSON strings.
- Keep JSON structure simple and consistent.

---

# Interview Questions

1. What is JSON?
2. Difference between JSON and JavaScript Objects?
3. What does JSON.stringify() do?
4. What does JSON.parse() do?
5. Why is JSON used in APIs?

---

# Summary

JSON is the standard format for exchanging data between web applications and servers. Every JavaScript developer should understand how to create, parse, and manipulate JSON data.
