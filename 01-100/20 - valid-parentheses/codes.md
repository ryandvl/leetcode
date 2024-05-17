# Codes

## JavaScript

```js
/**
 * @param {string} s
 * @return {boolean}
 */
var isValid = function (s) {
  let stack = [];

  for (var char of s) {
    if (["(", "[", "{"].includes(char)) {
      stack.push(char);
    } else {
      if(!stack.length) return false;

      const lastStack = stack[stack.length - 1];

      if (
        (lastStack != "(" && char == ")") ||
        (lastStack != "[" && char == "]") ||
        (lastStack != "{" && char == "}")
      ) {
        return false;
      }

      stack.pop();
    }
  }

  return !stack.length;
};
```


## Python

```py
class Solution:
    def isValid(self, s: str) -> bool:
        stack = []

        for char in s:
            if char in '([{':
                stack.append(char)
            else:
                if not stack return False

                if \
                    stack[-1] is not "(" and char is ")" or \
                    stack[-1] is not "[" and char is "]" or \
                    stack[-1] is not "{" and char is "}":
                    return False
                
                stack.pop()
                
        return not stack
```


## Java

```java
class Solution {
  public boolean isValid(String s) {
    Stack<Character> stack = new Stack<Character>();

    for (char c : s.toCharArray()) {
        if (c == '(' || c == '[' || c == '{') {
            stack.add(c);
        } else {
            if(stack.isEmpty()) return false;
            
            var lastStack = stack.get(stack.size() - 1);

            if ((lastStack != '(' && c == ')') ||
                (lastStack != '[' && c == ']') ||
                (lastStack != '{' && c == '}')) {
                    return false;
                }
            
            stack.pop();
        }
    }
            
    return stack.isEmpty();
  }
}
```


## C++

```cpp
class Solution {
public:
    bool isValid(string s) {
        stack<char> st;

        for (char c : s) {
            if (c == '(' || c == '[' || c == '{') {
                st.push(c);
            } else {
                if(st.empty()) return false;

                if (
                  (st.top() != '(' && c == ')') ||
                  (st.top() != '[' && c == ']') ||
                  (st.top() != '{' && c == '}')
                  )
                {
                  return false;
                }

              st.pop();
            }
        }
        
        return st.empty();
    }
};
```
