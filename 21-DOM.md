# JavaScript DOM (Document Object Model)

## Introduction

The DOM (Document Object Model) is a programming interface for HTML and XML documents. It represents a webpage as a tree of objects, allowing JavaScript to access, modify, add, or remove HTML elements dynamically.

Simply put:

> HTML creates the structure, CSS styles it, and JavaScript manipulates it through the DOM.

---

# Why is DOM Important?

Using the DOM, JavaScript can:

- Change HTML content
- Change CSS styles
- Add new HTML elements
- Remove existing elements
- Handle user events
- Validate forms
- Build interactive web applications

---

# DOM Tree

Example HTML

```html
<html>
    <body>
        <h1>Hello</h1>
        <p>Welcome</p>
    </body>
</html>
```

DOM Structure

```
Document
   |
 HTML
   |
 Body
  /  \
H1    P
```

---

# Selecting Elements

## getElementById()

```javascript
const heading = document.getElementById("title");
```

---

## getElementsByClassName()

```javascript
const items = document.getElementsByClassName("item");
```

---

## getElementsByTagName()

```javascript
const paragraphs = document.getElementsByTagName("p");
```

---

## querySelector()

Returns the first matching element.

```javascript
const button = document.querySelector(".btn");
```

---

## querySelectorAll()

Returns all matching elements.

```javascript
const buttons = document.querySelectorAll(".btn");
```

---

# Changing HTML Content

```javascript
document.getElementById("title").innerHTML = "Welcome to JavaScript";
```

---

# Changing Text

```javascript
document.getElementById("title").textContent = "Hello World";
```

---

# Changing CSS

```javascript
document.getElementById("title").style.color = "blue";

document.getElementById("title").style.fontSize = "40px";
```

---

# Changing Attributes

```javascript
const image = document.querySelector("img");

image.src = "cat.jpg";
```

---

# Creating Elements

```javascript
const para = document.createElement("p");

para.textContent = "New Paragraph";
```

---

# Adding Elements

```javascript
document.body.appendChild(para);
```

---

# Removing Elements

```javascript
const element = document.getElementById("old");

element.remove();
```

---

# Real-world Example

```javascript
const heading = document.getElementById("welcome");

heading.innerHTML = "Welcome Arul";
heading.style.color = "green";
```

---

# Best Practices

- Prefer querySelector() for flexibility.
- Avoid excessive DOM manipulation.
- Cache frequently used DOM elements.
- Separate JavaScript from HTML.

---

# Interview Questions

1. What is DOM?
2. Difference between HTML and DOM?
3. Difference between innerHTML and textContent?
4. Difference between querySelector() and querySelectorAll()?
5. How do you create an HTML element using JavaScript?

---

# Summary

The DOM allows JavaScript to interact with webpages dynamically by selecting, modifying, creating, and deleting HTML elements.
