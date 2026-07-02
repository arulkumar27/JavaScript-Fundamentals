# JavaScript Conditional Statements

## Introduction

Conditional statements allow programs to execute different code blocks based on specific conditions.

---

## if Statement

```javascript
let age = 20;

if(age >= 18){
    console.log("Eligible to Vote");
}
```

---

## if...else

```javascript
let marks = 45;

if(marks >= 50){
    console.log("Pass");
}
else{
    console.log("Fail");
}
```

---

## else if

```javascript
let score = 85;

if(score >= 90){
    console.log("Grade A");
}
else if(score >= 75){
    console.log("Grade B");
}
else{
    console.log("Grade C");
}
```

---

## Switch Statement

```javascript
let day = 2;

switch(day){
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    default:
        console.log("Invalid Day");
}
```

---

## Ternary Operator

```javascript
let age = 22;

let result = age >= 18 ? "Adult" : "Minor";

console.log(result);
```

---

## Real-world Example

Checking login status:

```javascript
let isLoggedIn = true;

if(isLoggedIn){
    console.log("Welcome");
}
else{
    console.log("Please Login");
}
```

---

## Best Practices

- Keep conditions simple.
- Use switch for multiple fixed options.
- Use meaningful comparisons.

---

## Interview Questions

1. Difference between if and switch?
2. What is a ternary operator?
3. Why use else if?
4. When should switch be used?
5. What happens if no condition matches?

---

## Summary

Conditional statements help applications make decisions based on user input or program logic.
