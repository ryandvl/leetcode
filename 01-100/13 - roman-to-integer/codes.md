# Codes

## JavaScript

```js
/**
 * @param {string} s
 * @return {number}
 */
var romanToInt = function (s) {
  const romans = {
    I: 1,
    V: 5,
    X: 10,
    L: 50,
    C: 100,
    D: 500,
    M: 1000,
  };

  let result = 0;

  for (let i = 0; i < s.length; ++i) {
    const currentRoman = romans[s[i]];
    const nextRoman = romans[s[i + 1]];

    if (currentRoman < nextRoman) {
      result -= currentRoman;
    } else {
      result += currentRoman;
    }
  }

  return result;
};
```


## Python

```py
class Solution:
    def romanToInt(self, s: str) -> int:
        romans = {
            "I": 1,
            "V": 5,
            "X": 10,
            "L": 50,
            "C": 100,
            "D": 500,
            "M": 1000
        }

        result = 0

        for i, current in enumerate(s):
            currentRoman = romans[current]
            
            if(i + 1 < len(s) and currentRoman < romans[s[i + 1]]):
                result -= currentRoman
            else:
                result += currentRoman

        return result
```


## Java

```java
class Solution {
    public int romanToInt(String s) {
        var romans = new HashMap<Character, Integer>() {{
            put('I', 1);
            put('V', 5);
            put('X', 10);
            put('L', 50);
            put('C', 100);
            put('D', 500);
            put('M', 1000);
        }};

        int result = 0;

        for (int i = 0; i < s.length(); i++) {
            var currentRoman = romans.get(s.charAt(i));
        
            if (
                i + 1 < s.length() &&
                currentRoman < romans.get(s.charAt(i + 1))
            ) {
                result -= currentRoman;
            } else {
                result += currentRoman;
            }
        }
      
        return result;
    }
}
```


## C++

```cpp
class Solution {
public:
    int romanToInt(string s) {
        unordered_map<char, int> romans = {
            {'I', 1},
            {'V', 5},
            {'X', 10},
            {'L', 50},
            {'C', 100},
            {'D', 500},
            {'M', 1000}
        };

        int result = 0;

        for (int i = 0; i < s.length(); ++i) {
          int currentRoman = romans[s[i]];
          int nextRoman = romans[s[i + 1]];

          if(currentRoman < nextRoman) {
            result -= currentRoman;
          } else {
            result += currentRoman;
          }
        }

        return result;
    }
};
```
