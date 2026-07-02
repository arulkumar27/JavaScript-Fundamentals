# JavaScript Loops

## Introduction

Loops execute a block of code repeatedly until a specified condition becomes false.

---

## for Loop

```javascript
for(let i = 1; i <= 5; i++){
    console.log(i);
}
```

---

## while Loop

```javascript
let i = 1;

while(i <= 5){
    console.log(i);
    i++;
}
```

---

## do...while Loop

```javascript
let i = 1;

do{
    console.log(i);
    i++;
}while(i <= 5);
```

---

## for...of Loop

Used for arrays and strings.

```javascript
let colors = ["Red","Blue","Green"];

for(let color of colors){
    console.log(color);
}
```

---

## for...in Loop

Used for object properties.

```javascript
let student = {
    name: "Arul",
    age: 22
};

for(let key in student){
    console.log(key, student[key]);
}
```

---

## break Statement

```javascript
for(let i = 1; i <= 10; i++){
    if(i == 6){
        break;
    }
    console.log(i);
}
```

---

## continue Statement

```javascript
for(let i = 1; i <= 5; i++){
    if(i == 3){
        continue;
    }
    console.log(i);
}
```

---

## Real-world Example

Displaying products in an e-commerce application:

```javascript
let products = ["Laptop", "Phone", "Tablet"];

for(let product of products){
    console.log(product);
}
```

---

## Best Practices

- Choose the appropriate loop for the task.
- Avoid infinite loops.
- Keep loop logic simple and readable.

---

## Interview Questions

1. Difference between `for` and `while`?
2. When do you use `for...of`?
3. What is `for...in` used for?
4. Explain `break` and `continue`.
5. How can infinite loops occur?

---

## Summary

Loops automate repetitive tasks such as processing arrays, displaying records, and handling repeated operations efficiently.
