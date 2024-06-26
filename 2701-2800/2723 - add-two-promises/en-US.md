# Problem

Given two promises `promise1` and `promise2`, return a new promise. `promise1` and `promise2` will both resolve with a number. The returned promise should resolve with the sum of the two numbers.

## Examples

> Input:
> ```
> promise1 = new Promise(resolve => setTimeout(() => resolve(2), 20)),
> promise2 = new Promise(resolve => setTimeout(() => resolve(5), 60))
> ```

> Output: `7`

> Explanation: The two input promises resolve with the values of `2` and `5` respectively. The returned promise should resolve with a value of `2 + 5 = 7`. The time the returned promise resolves is not judged for this problem.

** **

> Input:
> ```
> promise1 = new Promise(resolve => setTimeout(() => resolve(10), 50)), 
> promise2 = new Promise(resolve => setTimeout(() => resolve(-12), 30))
> ```

> Output: `-2`

> Explanation: The two input promises resolve with the values of `10` and `-12` respectively. The returned promise should resolve with a value of `10 + -12 = -2`.

## About my Solution

Use the `Promise.all` method on the two arrays to get the two input numbers, and then add them together.

### Key-points

- Use the `Promise.all` to get the expected result.

### Codes

> Languages in which I maked this Solution: `JavaScript` and `TypeScript`.

The codes are available in [codes.md](./codes.md).