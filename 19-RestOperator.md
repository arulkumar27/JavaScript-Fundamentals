# JavaScript Rest Operator

## Introduction

The Rest Operator (`...`) collects multiple values into a single variable. It is commonly used in function parameters and destructuring.

Although it uses the same syntax as the spread operator, its purpose is different.

---

## Syntax

```javascript
...
```

---

## Rest Parameters

```javascript
function sum(...numbers) {
    let total = 0;

    for (let number of numbers) {
        total += number;
    }

    return total;
}

console.log(sum(10, 20, 30, 40));
```

Output

```
100
```

---

## Array Destructuring

```javascript
const colors = ["Red", "Blue", "Green", "Yellow"];

const [first, ...remaining] = colors;

console.log(first);
console.log(remaining);
```

Output

```
Red
["Blue", "Green", "Yellow"]
```

---

## Object Destructuring

```javascript
const student = {
    name: "Arul",
    age: 22,
    city: "Salem"
};

const { name, ...details } = student;

console.log(name);
console.log(details);
```

---

## Real-world Example

```javascript
function shoppingCart(...items) {
    console.log(items);
}

shoppingCart(
    "Laptop",
    "Mouse",
    "Keyboard",
    "Monitor"
);
```

---

## Best Practices

- Use rest when the number of arguments is unknown.
- Rest parameter should always be the last parameter.
- Improves function flexibility.

---

## Interview Questions

1. What is the rest operator?
2. Difference between spread and rest?
3. Where can rest operator be used?
4. Why should rest be the last parameter?
5. Give a real-world example.

---

## Summary

The rest operator collects multiple values into one variable, making functions flexible and destructuring more powerful.
