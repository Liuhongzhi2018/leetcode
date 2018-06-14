#  Range Sum Query

## 问题分析
Given an integer array nums, find the sum of the elements between indices i and j (i ≤ j), inclusive.

给定一个整数数组  nums，求出数组从索引 i 到 j  (i ≤ j) 范围内元素的总和，包含 i,  j 两点。

## 代码实现
``` C
typedef struct{  
    int num;  
}NumArray;  
  
/** Initialize your data structure here. */  
struct NumArray* NumArrayCreate(int* nums, int numsSize) {  
    struct NumArray *obj=(struct NumArray*)malloc((struct NumArray)*numsSize);
    int i;
    obj[0].num = nums[0];  
    for(i = 1; i < numsSize; i++)  
    obj[i].num = nums[i] + obj[i-1].num;  
    return obj;  
}  
  
int sumRange(struct NumArray* obj, int i, int j) {  
    if(i == 0) return obj[j].num;  
    return obj[j].num - obj[i-1].num;  
} 
void NumArrayFree(struct NumArray* obj) {  
    free(obj);      
}

/**
 * Your NumArray struct will be instantiated and called as such:
 * struct NumArray* obj = numArrayCreate(nums, numsSize);
 * int param_1 = numArraySumRange(obj, i, j);
 * numArrayFree(obj);
 */
```

## 总结体会

本题需要求出在给定数组中从i到j范围内元素之和，需要了解题目所给各函数所要计算的内容。

struct NumArray* NumArrayCreate函数用来初始化数组obj，int sumRange用于求范围内之和，void NumArrayFree用于释放内存空间。
