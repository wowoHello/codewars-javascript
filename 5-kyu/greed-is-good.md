# Greed is Good <sup><sup>5 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/5270d0d18625160ada0000e4) - `ALGORITHMS`


## Description
Greed is a dice game played with five six-sided dice. Your mission, should you choose to accept it, is to score a throw according to these rules. You will always be given an array with five six-sided dice values.
```
 Three 1's => 1000 points
 Three 6's =>  600 points
 Three 5's =>  500 points
 Three 4's =>  400 points
 Three 3's =>  300 points
 Three 2's =>  200 points
 One   1   =>  100 points
 One   5   =>   50 point
```
A single die can only be counted once in each roll. For example, a given "5" can only count as part of a triplet (contributing to the 500 points) or as a single 50 points, but not both in the same roll.
<br /><br />
Example
```
Throw       Score
---------   ------------------
 5 1 3 4 1   250:  50 (for the 5) + 2 * 100 (for the 1s)
 1 1 1 3 1   1100: 1000 (for three 1s) + 100 (for the other 1)
 2 4 4 5 4   450:  400 (for three 4s) + 50 (for the 5)
```

## Solution
```javascript
function score( dice ) {
  let sum = 0
    for(i=1; i<=6; i++){
      const count = dice.filter( d => d == i).length
      if(count >= 3){
        sum += (i==1 ? 1000 : i*100)
      }
      if(i == 1){
        sum += (count % 3) * 100 
      }
      if(i == 5){
        sum += (count % 3) * 50
      }
    }
    return sum
}
```
