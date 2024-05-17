# Problem

Given a string `s` containing just the characters `'('`, `')'`, `'{'`, `'}'`, `'['` and `']'`, determine if the input string is valid.

An input string is valid if:

1. Open brackets must be closed by the same type of brackets.
2. Open brackets must be closed in the correct order.
3. Every close bracket has a corresponding open bracket of the same type.

## Examples

> Input: `s = "()"`

> Output: `true`

** **

> Input: `s = "()[]{}"`

> Output: `true`

** **

> Input: `s = "(]"`

> Output: `false`

## About my Solution

Scroll through the string and use the stack to store all characters that are any of these characters `([{` if the character is not one of these we enter another check where if the last element of the stack is not the opening key and the character is the closing key it returns false, if not just removing the last element from the array as it was successfully closed. In the end, we just need to check the size of the items in the stack, and if it's empty, we've succeeded.

### Key-points

- Reduce time to O(1) instead of O(N).

### Codes

> Languages in which I maked this Solution: `JavaScript`, `Python`, `Java` and `C++`.

The codes are available in [codes.md](./codes.md).