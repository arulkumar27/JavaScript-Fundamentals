# JavaScript Type Conversion

## Introduction

Type conversion is the process of changing one data type into another.

There are two types:

- Implicit Conversion
- Explicit Conversion

---

## Implicit Conversion

JavaScript automatically converts data types.

```javascript
"5" + 2
```

Output

```
52
```

---

## Explicit Conversion

Using Number()

```javascript
let value = "100";

let number = Number(value);

console.log(number);
```

---

## Convert to String

```javascript
let age = 25;

String(age);
```

---

## Convert to Boolean

```javascript
Boolean(1)
Boolean(0)
Boolean("")
Boolean("Hello")
```

---

## Parsing Numbers

```javascript
parseInt("100px")
```

Output

```
100
```

---

```javascript
parseFloat("45.67kg")
```

Output

```
45.67
```

---

## Real-world Example

A registration form receives age as text.

```javascript
let age = "22";

age = Number(age);

if(age >= 18){
    console.log("Eligible");
}
```

---

## Best Practices

- Always validate user input.
- Use Number() when converting numeric values.
- Avoid relying on automatic type conversion.

---

## Summary

Type conversion ensures data is processed correctly and prevents unexpected behavior in JavaScript applications.
