# JavaScript Events

## Introduction

Events are actions that occur in the browser, such as clicking a button, typing in a textbox, moving the mouse, or submitting a form.

JavaScript listens for these events and executes code in response.

---

# Why Events are Important

Events make websites interactive.

Examples:

- Login Button
- Search Box
- Shopping Cart
- Dropdown Menu
- Form Validation
- Image Slider

---

# Common Events

| Event | Description |
|--------|-------------|
| click | Mouse click |
| dblclick | Double click |
| mouseover | Mouse enters element |
| mouseout | Mouse leaves element |
| keydown | Key pressed |
| keyup | Key released |
| submit | Form submitted |
| change | Input value changed |
| focus | Input selected |
| blur | Input loses focus |

---

# Click Event

HTML

```html
<button id="btn">Click Me</button>
```

JavaScript

```javascript
const button = document.getElementById("btn");

button.addEventListener("click", function () {
    alert("Button Clicked");
});
```

---

# Mouseover Event

```javascript
const heading = document.querySelector("h1");

heading.addEventListener("mouseover", function () {
    heading.style.color = "red";
});
```

---

# Mouseout Event

```javascript
heading.addEventListener("mouseout", function () {
    heading.style.color = "black";
});
```

---

# Keydown Event

```javascript
document.addEventListener("keydown", function(event) {
    console.log(event.key);
});
```

---

# Change Event

```javascript
const input = document.querySelector("input");

input.addEventListener("change", function() {
    console.log(input.value);
});
```

---

# Submit Event

```javascript
const form = document.querySelector("form");

form.addEventListener("submit", function(event) {

    event.preventDefault();

    alert("Form Submitted");

});
```

---

# Event Object

```javascript
button.addEventListener("click", function(event){

    console.log(event);

});
```

---

# Real-world Example

```javascript
const loginButton = document.getElementById("login");

loginButton.addEventListener("click", function(){

    alert("Logging In...");

});
```

---

# Best Practices

- Use addEventListener().
- Avoid inline JavaScript.
- Remove unused event listeners.
- Use event.preventDefault() when required.

---

# Interview Questions

1. What is an event?
2. What is addEventListener()?
3. Difference between click and dblclick?
4. What is event.preventDefault()?
5. What is the Event Object?

---

# Summary

Events allow JavaScript to respond to user actions, making web applications dynamic and interactive.
