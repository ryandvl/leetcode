# Codes

## JavaScript

```js
/**
 * @param {number} x
 * @return {boolean}
 */
var isPalindrome = function (x) {
  if (x < 0) return false;

  const xString = x.toString();

  for (let i = 0; i < xString.length; i++) {
    const firstDigit = xString[i];
    const lastDigit = xString[xString.length - 1 - i];

    if (firstDigit !== lastDigit) {
      return false;
    }
  }

  return true;
};
```


## Python

```py
class Solution:
    def isPalindrome(self, x: int) -> bool:
        if x < 0:
            return False

        xString = str(x)

        for i, digit in enumerate(xString):
            firstDigit = xString[i]
            lastDigit = xString[len(xString) - 1 - i]

            if firstDigit is not lastDigit:
                return False
        
        return True
```


## Java

```java
class Solution {
    public boolean isPalindrome(int x) {
        if(x < 0) return false;

        String xString = Integer.toString(x);

        for (int i = 0; i < xString.length(); i++) {
            var firstDigit = xString.charAt(i);
            var lastDigit = xString.charAt(xString.length() - 1 - i);
        
            if (firstDigit != lastDigit) {
              return false;
            }
          }

        return true;
    }
}
```


## C++

```cpp
class Solution
{
public:
  bool isPalindrome(int x)
  {
    if (x < 0)
      return false;

    string xString = to_string(x);

    for (int i = 0; i < xString.length(); i++)
    {
      char firstDigit = xString[i];
      char lastDigit = xString[xString.length() - 1 - i];

      if (firstDigit != lastDigit)
      {
        return false;
      }
    }

    return true;
  }
};
```
