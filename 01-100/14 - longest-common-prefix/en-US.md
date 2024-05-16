# Problem

Write a function to find the longest common prefix string amongst an array of strings.

If there is no common prefix, return an empty string `""`.

## Examples

> Input: `strs = ["flower","flow","flight"]`

> Output: `"fl"`

** **

> Input: `strs = ["dog","racecar","car"]`

> Output: `""`

> Explanation: There is no common prefix among the input strings.

## About my Solution

The quickest solution I found has limitations but works depending on the elements, first we will use the `sort` method on the array to leave all elements in alphabetical order, so all elements that start with the same prefixes will be followed, after that we will go through each character of the first element and compare the first character of the first element with the first character of the last element, if they are different it will return "" because none was found, otherwise the character will be added to the result. The result is then returned.

### Key-points

- In this solution, the time must be O(n * m)

### Codes

> Languages in which I maked this Solution: `JavaScript`, `Python`, `Java` and `C++`.

The codes are available in [codes.md](./codes.md).