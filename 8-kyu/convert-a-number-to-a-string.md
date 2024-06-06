# Convert a Number to a String!<sup><sup>8 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/5265326f5fda8eb1160004c8) - `STRINGS` `FUNDAMENTALS`

## Description
We need a function that can transform a number (integer) into a string.

What ways of achieving this do you know?

**Examples (input --> output)**:
```
123  --> "123"
999  --> "999"
-100 --> "-100"
```

## Solution
```javascript
function numberToString(num) {
  return num.toString();
}
```