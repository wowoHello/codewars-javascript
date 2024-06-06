# Highest and Lowest<sup><sup>7 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/554b4ac871d6813a03000035) - `STRINGS` `FUNDAMENTALS`

## Description
In this little assignment you are given a string of space separated numbers, and have to return the highest and lowest number.

**Examples**
```
highAndLow("1 2 3 4 5");  // return "5 1"
highAndLow("1 2 -3 4 5"); // return "5 -3"
highAndLow("1 9 3 4 -5"); // return "9 -5"
```
**Notes**
* All numbers are valid `Int32`, no need to validate them.
* There will always be at least one number in the input string.
* Output string must be two numbers separated by a single space, and highest number is first.

## Solution
```javascript
function highAndLow(numbers){
  let arrNum = numbers.split(' ');
  let numMax = Math.max(...arrNum);
  let numMin = Math.min(...arrNum);
  return numMax + ' ' + numMin;
}
```