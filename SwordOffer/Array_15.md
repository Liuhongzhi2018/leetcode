# 滑动窗口的最大值


## 题目描述

给定一个数组和滑动窗口的大小，找出所有滑动窗口里数值的最大值。例如，如果输入数组{2,3,4,2,6,2,5,1}及滑动窗口的大小3，那么一共存在6个滑动窗口，他们的最大值分别为{4,4,6,6,6,5}； 针对数组{2,3,4,2,6,2,5,1}的滑动窗口有以下6个： {[2,3,4],2,6,2,5,1}， {2,[3,4,2],6,2,5,1}， {2,3,[4,2,6],2,5,1}， {2,3,4,[2,6,2],5,1}， {2,3,4,2,[6,2,5],1}， {2,3,4,2,6,[2,5,1]}。


## 代码实现

1. 
```python
# -*- coding:utf-8 -*-
class Solution:
    def maxInWindows(self, num, size):
        # write code here
        if not num: 
            return [] 
        if size > len(num) or size < 1: 
            return [] 
        if size == 1: 
            return num 
        temp = [0] 
        res = [] 
        for i in range(len(num)): 
            if i - temp[0] > size - 1: 
                temp.pop(0) 
            while len(temp) > 0 and num[i] >= num[temp[-1]]: 
                temp.pop() 
            temp.append(i) 
            if i >= size - 1: 
                res.append(num[temp[0]]) 
        return res
```
运行时间：30ms

占用内存：5624k


## 思路总结

建立一个列表存储最大值的变化，列表首位为目前最大值的坐标，之后为次大值等。当新来一个数时，首先判断原来老大是否还管的到这里，管不到则弹出。新来的逐个与前面的值比较，比他小的就没有话语权了，直接弹出。若全都比过，弹出了，新来的就是老大。若中间存在比不过的就存在队尾端，等待前面的人老去，管不到后边。或者本来就有空位，或者老大老去，所以新来的总是有位置的。