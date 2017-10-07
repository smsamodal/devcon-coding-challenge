# Coin Change Problem

You have different types of coins available in infinite quantities where the value of each coin is given in the array *C = [C0, C1, ... , Cm-1]*. Determine all possible ways of making change using the given types of coins. For example, if *Change = 4*, and *C = [8, 3, 1, 2]*, we can make change in three ways: *{1, 1, 1}*, *{1, 2}*, and *{3}*. Feel free to use any programming language though the prefered is Javascript.

Constraints:
- Coin values is between the range 1-50
- Each coin value in the array is guaranteed to be distinct

Function Format:

```
function coinChange(change, coins) {
   return [];
}
```

Input 0
```
Coins = [1, 2, 3]
Change = 4
```

Output 0
```
[
  [1, 1, 1, 1],
  [1, 1, 2],
  [2, 2],
  [1, 3]
]
```

----

Input 1
```
Coins = [2, 5, 3, 6]
Change = 10
```

Output 1
```
[
  [2, 2, 2, 2, 2],
  [2, 2, 3, 3],
  [2, 2, 6],
  [2, 3, 5],
  [5, 5]
]
```
