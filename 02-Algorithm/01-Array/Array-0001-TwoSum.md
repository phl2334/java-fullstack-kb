---
tags: [algorithm, array]
difficulty: Easy
topic: 哈希表
status: solved
leetcode_url: "https://leetcode.cn/problems/two-sum/"
created: 2026-08-31
last_review: 
next_review: 2026-09-03
---

# Array-0001-TwoSum

## 题目描述
给定一个整数数组 `nums` 和一个整数目标值 `target`，请你在该数组中找出和为目标值 `target` 的那两个整数，并返回它们的数组下标。

## 解题思路

### 第一步：理解题意（3-5分钟）
- 输入：数组 nums，目标值 target
- 输出：两个数的下标
- 约束：每种输入只会对应一个答案，同一个元素不能使用两遍
- 例子：nums=[2,7,11,15], target=9 → 返回 [0,1]

### 第二步：暴力解法
- 思路：两层循环，枚举所有两数组合
- 复杂度：时间 O(n²)，空间 O(1)
- 为什么不行？n 大了会超时

### 第三步：优化思路
- 瓶颈：找 `target - nums[i]` 是否在数组里
- 优化：用 HashMap 存已经遍历过的数，一次遍历搞定
- 验证：遍历到 7 时，map 里已经有 2，9-7=2 存在，返回下标

## 代码（Java）

```java
class Solution {
    public int[] twoSum(int[] nums, int target) {
        Map<Integer, Integer> map = new HashMap<>();
        for (int i = 0; i < nums.length; i++) {
            int complement = target - nums[i];
            if (map.containsKey(complement)) {
                return new int[] { map.get(complement), i };
            }
            map.put(nums[i], i);
        }
        return new int[0];
    }
}
```

## 复杂度分析
| 指标 | 复杂度 | 说明 |
|------|--------|------|
| 时间 | O(n) | 只遍历一次数组 |
| 空间 | O(n) | HashMap 最多存 n 个数 |

## 复盘记录
| 次数 | 日期 | 状态 | 卡壳点 |
|------|------|------|--------|
| 1 | 2026-08-31 | ✅ | 无，第一题很顺 |
| 2 | | | |
| 3 | | | |

## 相关题目
- [[Array-0167-TwoSumII]] — 数组已排序，用双指针
- [[HashTable-0001-TwoSum]] — 同一道题，归类到哈希表

## 面试口述稿
这道题用哈希表来做。我们遍历数组，对于每个数，先检查 `target - 当前数` 是否在哈希表里，如果在就返回两个下标；如果不在，就把当前数和下标放进哈希表。时间复杂度 O(n)，空间复杂度 O(n)。
