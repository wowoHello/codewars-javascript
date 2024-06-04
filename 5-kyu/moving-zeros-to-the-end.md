# Moving Zeros To The End<sup><sup>5 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/52597aa56021e91c93000cb0) - `ARRAYS` `SORTING` `ALGORITHMS`

## Description
Write an algorithm that takes an array and moves all of the zeros to the end, preserving the order of the other elements.
```
moveZeros([false,1,0,1,2,0,1,3,"a"]) // returns[false,1,1,2,1,3,"a",0,0]
```

## Solution
```javascript
function moveZeros(arr) {
    let a = arr.filter( e => e !== 0);
    let b = arr.filter( e => e === 0);
    return a.concat(b);
}
```