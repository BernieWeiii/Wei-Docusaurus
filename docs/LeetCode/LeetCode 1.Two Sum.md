# [LeetCode] 1.Two Sum 解題過程

程式語言:JavaScript

1.Two Sum

題目敘述：Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.You may assume that each input would have exactly one solution, and you may not use the same element twice.You can return the answer in any order.

Example1:

```
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
```

Example2:

```
Input: nums = [3,2,4], target = 6
Output: [1,2]
```

Example3:

```
Input: nums = [3,3], target = 6
Output: [0,1]
```

作為解題的一開始，還是要從最經典的 Two Sum 作為開頭吧！
最直覺的作法就是使用雙迴圈走完整個陣列，把值相加起來等於 target 的 index 回傳回來。

時間複雜度:O(n^2)

```js showLineNumbers
var twoSum = function (nums, target) {
  for (let i = 0; i < nums.length; i++) {
    for (let j = i + 1; j < nums.length; j++) {
      if (nums[i] + nums[j] == target) {
        return [i, j];
      }
    }
  }
};
```

日期:2023-03-28
<br/>
今天的解題就結束囉，明天讓我們繼續。
