# Codes

## JavaScript

```js
/**
 * @param {string[]} strs
 * @return {string}
 */
var longestCommonPrefix = function (strs) {
  strs.sort();

  const firstStr = strs[0];
  const lastStr = strs[strs.length - 1];

  let result = "";

  for (let i = 0; i < firstStr.length; i++) {
    const firstChar = firstStr[i];
    const lastChar = lastStr[i];

    if (firstChar != lastChar) {
      break;
    } else {
      result += firstChar;
    }
  }

  return result;
};
```


## Python

```py
class Solution:
    def longestCommonPrefix(self, strs: list[str]) -> str:
        strs.sort()
        
        firstStr = strs[0]
        lastStr = strs[-1]

        result = ""

        for i, current in enumerate(firstStr):
            firstChar = firstStr[i]
            lastChar = lastStr[i]

            if firstChar is not lastChar:
                break
            else:
                result += firstChar

        return result
```


## Java

```java
class Solution {
    public String longestCommonPrefix(String[] strs) {
        Arrays.sort(strs);

        String firstStr = strs[0];
        String lastStr = strs[strs.length - 1];
      
        var result = new StringBuilder();
      
        for (int i = 0; i < firstStr.length(); i++) {
          var firstChar = firstStr.charAt(i);
          var lastChar = lastStr.charAt(i);
      
          if (firstChar != lastChar) {
            break;
          } else {
            result.append(firstChar);
          }
        }
      
        return result.toString();
    }
}
```


## C++

```cpp
class Solution
{
public:
    string longestCommonPrefix(vector<string> &strs)
    {
      sort(strs.begin(), strs.end());

      string firstStr = strs.front();
      string lastStr = strs.back();

      string result = "";

      for (int i = 0; i < firstStr.length(); i++)
      {
        char firstChar = firstStr.at(i);
        char lastChar = lastStr.at(i);

        if(firstChar != lastChar) {
          break;
        } else {
          result += firstChar;
        }
      }

      return result;
    }
};
```
