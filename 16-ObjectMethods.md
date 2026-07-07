# JavaScript Object Methods

## Introduction

JavaScript provides several built-in methods to work with objects efficiently. These methods help retrieve object keys, values, entries, copy objects, freeze objects, and more.

---

## Why Use Object Methods?

Object methods make it easier to:

- Access object properties
- Copy objects
- Merge objects
- Prevent object modification
- Iterate through object data

---

## Object.keys()

Returns an array containing all property names.

```javascript
const student = {
    name: "Arul",
    age: 22,
    city: "Salem"
};

console.log(Object.keys(student));
```

Output

```
["name", "age", "city"]
```

---

## Object.values()

Returns all property values.

```javascript
console.log(Object.values(student));
```

Output

```
["Arul", 22, "Salem"]
```

---

## Object.entries()

Returns key-value pairs.

```javascript
console.log(Object.entries(student));
```

Output

```
[
 ["name","Arul"],
 ["age",22],
 ["city","Salem"]
]
```

---

## Object.assign()

Copies or merges objects.

```javascript
const address = {
    state: "Tamil Nadu"
};

const details = Object.assign({}, student, address);

console.log(details);
```

Output

```
{
 name: "Arul",
 age: 22,
 city: "Salem",
 state: "Tamil Nadu"
}
```

---

## Object.freeze()

Prevents modifications.

```javascript
const user = {
    name: "Arul"
};

Object.freeze(user);

user.name = "Kumar";

console.log(user.name);
```

Output

```
Arul
```

---

## Object.seal()

Allows updating existing properties but prevents adding or deleting properties.

```javascript
const product = {
    name: "Laptop",
    price: 50000
};

Object.seal(product);

product.price = 55000;

console.log(product);
```

---

## Real-world Example

```javascript
const employee = {
    id: 101,
    name: "Arul",
    department: "IT"
};

console.log(Object.keys(employee));
console.log(Object.values(employee));
```

---

## Best Practices

- Use Object.keys() for iteration.
- Use Object.assign() or the spread operator for copying objects.
- Use Object.freeze() for constant configuration objects.
- Avoid modifying shared objects directly.

---

## Interview Questions

1. What does Object.keys() return?
2. Difference between Object.values() and Object.entries()?
3. What is Object.assign()?
4. Difference between Object.freeze() and Object.seal()?
5. How do you copy an object?

---

## Summary

Object methods provide efficient ways to inspect, copy, merge, and protect JavaScript objects.
