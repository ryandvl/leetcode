# Codes

## JavaScript

```js
/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {
    const hashmap = new Map();

    for (let i = 0; i < nums.length; i++) {
      const x = target - nums[i];

      if(hashmap.has(x)) {
        return [hashmap.get(x), i];
      }

      hashmap.set(nums[i], i);
    }

    return [];
};
```


## Python

```py
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        hashmap = dict()

        for i, num in enumerate(nums):
            x = target - num

            if x in hashmap:
                return [hashmap[x], i]
            
            hashmap[num] = i

        return []
```


## Java

```java
class Solution {
    public int[] twoSum(int[] nums, int target) {
        var hashmap = new HashMap<Integer, Integer>();

        for (int i = 0; i < nums.length; i++) {
            var x = target - nums[i];

            if(hashmap.containsKey(x)) {
                return new int[]{hashmap.get(x), i};
            }

            hashmap.put(nums[i], i);
        }

        return new int[0];
    }
}
```


## C++

```cpp
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        unordered_map<int, int> hashmap;

        for (int i = 0; i < nums.size(); ++i) {
          int x = target - nums[i];

          if(hashmap.find(x) != hashmap.end()) {
            return {hashmap[x], i};
          }

          hashmap[nums[i]] = i;
        }

        return {};
    }
};
```
