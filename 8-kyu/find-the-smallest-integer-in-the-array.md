# Find the smallest integer in the array<sup><sup>8 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/55a2d7ebe362935a210000b2) - `FUNDAMENTALS`

## Description
Given an array of integers your solution should find the smallest integer.

For example:
```
* Given [34, 15, 88, 2] your solution will return 2
* Given [34, -345, -1, 100] your solution will return -345
```
You can assume, for the purpose of this kata, that the supplied array will not be empty.


## Solution
```javascript
function findSmallestInt(arr) {
  return Math.min(...arr);
}
```