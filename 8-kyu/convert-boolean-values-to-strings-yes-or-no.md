# Convert boolean values to strings 'Yes' or 'No'<sup><sup>8 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/53369039d7ab3ac506000467) - `FUNDAMENTALS`

## Description
Complete the method that takes a boolean value and return a `"Yes"` string for `true`, or a `"No"` string for `false`.

## Solution
```javascript
function boolToWord( bool ){
  return bool == true ? "Yes" : "No";
}
```