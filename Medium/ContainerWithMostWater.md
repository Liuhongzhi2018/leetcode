#  Container With Most Water

## 问题分析
Given n non-negative integers a1, a2, ..., an, where each represents a point at coordinate (i, ai). n vertical lines are drawn such that the two endpoints of line i is at (i, ai) and (i, 0). Find two lines, which together with x-axis forms a container, such that the container contains the most water.

Note: You may not slant the container and n is at least 2. 

给定 n 个非负整数 a1，a2，...，an，每个数代表坐标中的一个点 (i, ai) 。画 n 条垂直线，使得垂直线 i 的两个端点分别为 (i, ai) 和 (i, 0)。找出其中的两条线，使得它们与 x 轴共同构成的容器可以容纳最多的水。

注意：不能倾斜容器，n 至少是2。


## 代码实现
``` C
int maxArea(int* height, int heightSize) {
    int i=0;
    int j=heightSize-1;
    int area,water=0;
    while(i<j){
        if(height[i]<height[j]){
            area=height[i]*(j-i);
            i++;
        }
        else{
            area=height[j]*(j-i);
            j--;
        }
        if(water<area)  water=area;
    }
        return water;
}
```

## 总结体会

本题要求能盛水的最大容器，可以转换为计算矩形的面积，长度为横坐标间距，宽度取决于最小边，找出符合条件两点，返回最大面积。

在算法设计上，首先将组成矩形的左右两点坐标定义为i和j，起始位置分别对应最左和最右点；其次采用while循环，确定最短边长，使i和j依次向中间递进，并计算矩形面积；最后比较得到最大的面积返回。


