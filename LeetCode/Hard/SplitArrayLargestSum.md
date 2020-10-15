#   Split Array Largest Sum

## 问题描述

Given an array nums which consists of non-negative integers and an integer m, you can split the array into m non-empty continuous subarrays.

Write an algorithm to minimize the largest sum among these m subarrays.

给定一个非负整数数组和一个整数 m，你需要将这个数组分成 m 个非空的连续子数组。设计一个算法使得这 m 个子数组各自和的最大值最小。

注意:  
数组长度 n 满足以下条件:

    1 ≤ n ≤ 1000
    1 ≤ m ≤ min(50, n)




## 代码实现

1.二分查找
```python
class Solution:
    def splitArray(self, nums: List[int], m: int) -> int:
        l, r = max(nums), sum(nums)

        def gs(mid):
            cnt, sums = 1, 0
            for i in nums:
                if sums + i > mid:
                    cnt += 1
                    sums = i
                else:
                    sums += i

            return cnt

        while l < r:
            mid = l + (r-l)//2
            if gs(mid) <= m:
                r = mid
            else:
                l = mid + 1
        return l
```


## 思路总结

二分查找的通常思路

    如果做多了二分查找的题，这道题应该会有思路。
    我们二分查找的时候，关键是要抓到施以查找的变量。即我们的left,right 和 mid 表示的是什么。
    对于简单题，往往就是列表的一项。比如对一个排序好的列表找到一个相应的值的位置，那么我们要施以查找的变量就是列表的下标，而缩小范围的依据就是列表的值。
    对于复杂的题，往往这个施以查找的变量会比较难抓。它往往不是列表里的一个项，而是一个要输出的值或判断依据做相应的变换。
    难点就在于划分出哪些是施以查找的变量，哪些是这些变量的更新准则。

针对这题的二分查找思路

    那么，对于这题，施以查找的变量是什么呢？
    我们注意到题目里说的m个子数组各自和的最大值最小。
    这是一个判断依据，也可以作为我们的施以查找的变量。
    显然，如果对这个数组，每个数单独成一数组，那么子数组的各自和的最大值，就是所有数中的最大值。
    而如果对这个数组不分组，那么子数组的各自和的最大值就是这个数组的和。
    这两个值对应的就是 left 和 right，即全分组与不分组的结果。
    套有我认为非常不错的这套「二分查找模板」，可以很容易写出这样的代码。

更新依据

    刚刚的注释里写道 排除右侧的条件
    怎样排除左侧的条件呢？即，给定一个左，右，和中间值，如何判断我们需要的最大值在中间和左边围起来的范围内呢？
    我们假设给定了mid，那么需要判断，如果以mid作为最大值，能形成几组，然后和给定的m值作对比。显然，如果这个mid越大，要分出来的组数越少。
    如果形成的组数比要求的多，说明这个给定的mid太小了，要扩大，而如果形成的组数太少了，说明给定的mid太大了，要缩小。
    而如果相等呢？我们假设有这么一个题目，给定列表[5,123]和m = 2来找出最大值，假如在二分中选择了124，这样子只能分成两个组，而显然124这个数不是正确答案，正确答案是123，所以相等的时候，我们认为这个查找值mid应该缩小。
    如果设定一个cnt变量记录分组数，即可写成这样的形式。
    
计算cnt的方法

    可是分组数怎么计算呢？
    思路是这样，我们维护一个cnt和一个sums，表示目前的组数和目前的和。
    初始，自然cnt = 1，sums = 0
    我们遍历这个数组
        让sums加上这个遍历着的数
        如果这个加起来的和比上限要小，那么就遍历下一个
        如果这个加起来的和比上限大，说明要分组了
        那么cnt += 1，同时这个数作为新组的开头，即sums = 这个遍历的数