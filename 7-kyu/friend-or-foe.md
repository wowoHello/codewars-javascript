# Friend or Foe?<sup><sup>7 Kyu</sup></sup>
[LINK TO THE KATA](https://www.codewars.com/kata/55b42574ff091733d900002f) - `FUNDAMENTALS`

## Description
Make a program that filters a list of strings and returns a list with only your friends name in it.

If a name has exactly 4 letters in it, you can be sure that it has to be a friend of yours! Otherwise, you can be sure he's not...

Ex: Input = ["Ryan", "Kieran", "Jason", "Yous"], Output = ["Ryan", "Yous"]
```
friend ["Ryan", "Kieran", "Mark"] `shouldBe` ["Ryan", "Mark"]
```
Note: keep the original order of the names in the output.

## Solution
```javascript
function friend(friends){
  return friends.filter( e => e.length === 4);
}
```