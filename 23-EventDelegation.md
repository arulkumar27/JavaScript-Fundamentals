# JavaScript Event Delegation

## Introduction

Event Delegation is a technique where you attach a single event listener to a parent element instead of adding event listeners to multiple child elements.

This works because of **Event Bubbling**, where an event starts from the target element and bubbles up through its parent elements.

---

# Why Use Event Delegation?

Benefits include:

- Improves performance
- Reduces memory usage
- Handles dynamically created elements
- Cleaner and more maintainable code

---

# Without Event Delegation

```javascript
const buttons = document.querySelectorAll(".btn");

buttons.forEach(button => {
    button.addEventListener("click", () => {
        console.log("Button Clicked");
    });
});
```

---

# With Event Delegation

```javascript
const container = document.getElementById("container");

container.addEventListener("click", function(event) {

    if(event.target.classList.contains("btn")){
        console.log("Button Clicked");
    }

});
```

---

# HTML Example

```html
<div id="container">

    <button class="btn">Button 1</button>

    <button class="btn">Button 2</button>

    <button class="btn">Button 3</button>

</div>
```

---

# Event Bubbling

When Button 1 is clicked:

```
Button
   ↑
Div
   ↑
Body
   ↑
HTML
   ↑
Document
```

The event moves upward through parent elements.

---

# Event Target

```javascript
container.addEventListener("click", function(event){

    console.log(event.target);

});
```

---

# Real-world Example

Imagine an online shopping website where products are loaded dynamically.

Instead of attaching click events to every "Add to Cart" button, attach one listener to the product container and detect which button was clicked.

---

# Best Practices

- Use Event Delegation for large lists.
- Check `event.target` before performing actions.
- Avoid attaching hundreds of individual event listeners.
- Use `closest()` when needed to find parent elements.

---

# Interview Questions

1. What is Event Delegation?
2. Why is Event Delegation useful?
3. What is Event Bubbling?
4. What is `event.target`?
5. When should Event Delegation be used?

---

# Summary

Event Delegation improves performance by attaching a single event listener to a parent element, making applications faster and easier to maintain.
