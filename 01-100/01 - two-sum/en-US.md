# Problem

Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

## Examples

> Input: `nums = [2,7,11,15], target = 9`

> Output: `[0,1]`

> Explanation: Because `nums[0] + nums[1] == 9`, we return `[0, 1]`.

** **

> Input: `nums = [3,2,4], target = 6`

> Output: `[1,2]`

** **

> Input: `nums = [3,3], target = 6`

> Output: `[0,1]`

## About my Solution

The easiest solution is to go through the entire array once, and during the process save the numbers in something like Hashmap, if the difference between the number and the target is found in the Hashmap, and in the final step, if found, returns `index of number found, current index`, the result was found.

### Key-points

- When going through `nums` we can use `target - num` to detect if there is a number that, added to the current one, will be the `target`.
- Use Hashmap to save the indexes of numbers that have already been covered.
- Reduce time to O(1) instead of O(N).

### Codes

> Languages in which I maked this Solution: `JavaScript`, `Python`, `Java` and `C++`.

The codes are available in [codes.md](./codes.md).