# Problem

Given an integer `x`, return `true` if `x` is a **palindrome**, and `false` otherwise.

An integer is a palindrome when it reads the same forward and backward.

For example, `121` is a palindrome while `123` is not.

## Examples

> Input: `x = 121`

> Output: `true`

> Explanation: `121` reads as `121` from `left to right` and from `right to left`.

** **

> Input: `x = -121`

> Output: `false`

> Explanation: From `left to right`, it reads `-121`. From `right to left`, it becomes `121-`. Therefore it is not a **palindrome**.

** **

> Input: `x = 10`

> Output: `false`

> Explanation: Reads `01` from `right to left`. Therefore it is not a **palindrome**.

## About my Solution

Scrolling through each digit of the whole number, at each index we check if the index of the opposite order is the same as the current one, so we can return `false` directly if they are not the same, and numbers smaller than `0` will always be `false`.

### Key-points

- We can check that the digit `size of x` minus the `current index` are the same digits.
- Reduce time to O(1) instead of O(N).

### Codes

> Languages in which I maked this Solution: `JavaScript`, `Python`, `Java` and `C++`.

The codes are available in [codes.md](./codes.md).