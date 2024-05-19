# Codes

## JavaScript

```js
/**
 * @param {Promise} promise1
 * @param {Promise} promise2
 * @return {Promise}
 */
var addTwoPromises = async function(promise1, promise2) {
    const [x, y] = await Promise.all([promise1, promise2]);

    return x + y;
};
```


## TypeScript

```ts
type P = Promise<number>

async function addTwoPromises(promise1: P, promise2: P): P {
    const [x, y]: [number, number] = await Promise.all([promise1, promise2]);

    return x + y;
};
```
