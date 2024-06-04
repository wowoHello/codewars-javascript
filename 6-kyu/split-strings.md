# Split Strings<sup><sup>6 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/515de9ae9dcfc28eb6000001) - `REGULAR EXPRESSIONS` `STRINGS` `ALGORITHMS`

## Description
Complete the solution so that it splits the string into pairs of two characters. If the string contains an odd number of characters then it should replace the missing second character of the final pair with an underscore ('_').

Examples:
```
* 'abc' =>  ['ab', 'c_']
* 'abcdef' => ['ab', 'cd', 'ef']
```

## Solution
```javascript
function solution(str){
   let arr = str.split('')
   let res = []

   for(let i = 0; i<arr.length; i+=2){
     if(arr[i+1]) res.push(arr[i]+arr[i+1])
     else res.push(arr[i]+'_')
   }

  return res
}
```