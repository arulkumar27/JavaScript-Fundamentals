# JavaScript Objects

## Introduction

Objects store data as key-value pairs and are used to represent real-world entities.

---

## Creating an Object

```javascript
const student = {
    name: "Arul",
    age: 22,
    city: "Salem"
};
```

---

## Accessing Properties

```javascript
console.log(student.name);
console.log(student["age"]);
```

---

## Updating Properties

```javascript
student.city = "Chennai";
```

---

## Adding Properties

```javascript
student.course = "JavaScript";
```

---

## Deleting Properties

```javascript
delete student.age;
```

---

## Object Methods

```javascript
const person = {
    name: "Arul",

    greet() {
        console.log("Hello");
    }
};

person.greet();
```

---

## Real-world Example

```javascript
const employee = {
    id: 101,
    name: "Arul",
    department: "IT",
    salary: 45000
};

console.log(employee);
```

---

## Best Practices

- Use descriptive property names.
- Group related data together.
- Keep object structures simple.

---

## Interview Questions

1. What is an object?
2. Difference between arrays and objects?
3. How do you access object properties?
4. How do you delete a property?
5. What are object methods?

---

## Summary

Objects are used extensively to model users, products, employees, and other real-world entities.
