# 剑指Offer

## 学习文档

[数据结构](https://www.bilibili.com/video/av86803650?from=search&seid=1397237482083708915)

[剑指offer-数据结构与算法](https://www.bilibili.com/video/av64288683/?spm_id_from=333.788.videocard.2)


## 题目清单


### 数组 (Array) (11道)：

数组是最简单的一种数据结构，它占据一块连续的内存并按照顺序存储数据。创建数组时需要首先指定数组的容量大小，然后根据大小分配内存，即使只在数组中存储一个数组，也需要为所有的数据预先分配内存，因此空间效率不高，但是时间效率高。

根据时间效率高的优点可用数组实现简单的哈希表，数组下标设为哈希表的键值Key，数组的元素设为哈希表的值Value，组成一个键值-值配对。

解决数组空间效率不高的问题可设计动态数组。先开辟小空间添加数据，当数目超过数组容量时重新分配更大空间，之前数据复制到新数组，释放之前的内存。

在C/C++中数组和指针相互关联又区别，当声明数组时，数组名也是一个指针，指针指向数组的第一个元素，访问元素时，要确保没有超出数组的边界。

* [剑指Offer（一）：二维数组中的查找](http://cuijiahua.com/blog/2017/11/basis_1.html)
* [剑指Offer（六）：旋转数组的最小数字](http://cuijiahua.com/blog/2017/11/basis_6.html)
* [剑指Offer（十三）：调整数组顺序使奇数位于偶数前面](http://cuijiahua.com/blog/2017/11/basis_13.html)
* [剑指Offer（二十八）：数组中出现次数超过一半的数字](http://cuijiahua.com/blog/2017/12/basis_28.html)
* [剑指Offer（三十）：连续子数组的最大和](http://cuijiahua.com/blog/2017/12/basis_30.html)
* [剑指Offer（三十二）：把数组排成最小的数](http://cuijiahua.com/blog/2018/01/basis_32.html)
* [剑指Offer（三十五）：数组中的逆序对](http://cuijiahua.com/blog/2018/01/basis_35.html)
* [剑指Offer（三十七）：数字在排序数组中出现的次数](http://cuijiahua.com/blog/2018/01/basis_37.html)
* [剑指Offer（四十）：数组中只出现一次的数字](http://cuijiahua.com/blog/2018/01/basis_40.html)
* [剑指Offer（五十）：数组中重复的数字](http://cuijiahua.com/blog/2018/01/basis_50.html)
* [剑指Offer（五十一）：构建乘积数组](http://cuijiahua.com/blog/2018/01/basis_51.html)


|                  Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|     二维数组中的查找                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_1.md) | |
|     数组中重复的数字                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_2.md) | |
|     构建乘积数组                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_3.md) | |
|      旋转数组的最小数字                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_4.md) | |
|      调整数组顺序使奇数位于偶数前面                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_5.md) | |
|      数组中出现次数超过一半的数字                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_6.md) | |
|      数组中只出现一次的数字                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_7.md) | |
|      最小的K个数                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_8.md) | |
|      连续子数组的最大和                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_9.md) | |
|      顺时针打印矩阵                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_10.md) | |
|      字符串的排列                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_11.md) | |
|      把数组排成最小的数                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_12.md) | |
|      数组中的逆序对                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_13.md) | |
|      数字在排序数组中出现的次数                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_14.md) | |
|      滑动窗口的最大值                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Array_15.md) | |


### 字符串 (String) (8道):

字符串是由若干字符组成的序列。

* [剑指Offer(二)：替换空格](http://cuijiahua.com/blog/2017/11/basis_2.html "悬停显示")
* [剑指Offer（二十七）：字符串的排列](http://cuijiahua.com/blog/2017/12/basis_27.html "悬停显示")
* [剑指Offer（三十四）：第一个只出现一次的字符](http://cuijiahua.com/blog/2018/01/basis_34.html "悬停显示")
* [剑指Offer（四十三）：左旋转字符串](http://cuijiahua.com/blog/2018/01/basis_43.html "悬停显示")
* [剑指Offer（四十四）：翻转单词顺序序列](http://cuijiahua.com/blog/2018/01/basis_44.html "悬停显示")
* [剑指Offer（四十九）：把字符串转换成整数](http://cuijiahua.com/blog/2018/01/basis_49.html "悬停显示")
* [剑指Offer（五十二）：正则表达式匹配](http://cuijiahua.com/blog/2018/01/basis_52.html "悬停显示")
* [剑指Offer（五十三）：表示数值的字符串](http://cuijiahua.com/blog/2018/01/basis_53.html "悬停显示")

|                  Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|     替换空格                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_1.md) | |
|     正则表达式匹配                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_2.md) | |
|     表示数值的字符串                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_3.md) | |
|     字符流中第一个不重复的字符                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_4.md) | |
|     第一个只出现一次的字符                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_5.md) | |
|     左旋转字符串                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_6.md) | |
|     翻转单词顺序序列                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_7.md) | |
|     扑克牌顺子                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_8.md) | |
|     把字符串转换成整数                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/String_9.md) | |

### 链表 (LinkedList) (8道)


* [剑指Offer（三）：从尾到头打印链表](http://cuijiahua.com/blog/2017/11/basis_3.html "悬停显示")
* [剑指Offer（十四）：链表中倒数第k个结点](http://cuijiahua.com/blog/2017/12/basis_14.html "悬停显示")
* [剑指Offer（十五）：反转链表](http://cuijiahua.com/blog/2017/12/basis_15.html "悬停显示")
* [剑指Offer（十六）：合并两个排序的链表](http://cuijiahua.com/blog/2017/12/basis_16.html "悬停显示")
* [剑指Offer（二十五）：复杂链表的复制](http://cuijiahua.com/blog/2017/12/basis_25.html "悬停显示")
* [剑指Offer（三十六）：两个链表的第一个公共结点](http://cuijiahua.com/blog/2018/01/basis_36.html "悬停显示")
* [剑指Offer（五十五）：链表中环的入口结点](http://cuijiahua.com/blog/2018/01/basis_55.html "悬停显示")
* [剑指Offer（五十六）：删除链表中重复的结点](http://cuijiahua.com/blog/2018/01/basis_56.html "悬停显示")
* [剑指Offer（四十六）：孩子们的游戏（圆圈中最后剩下的数）](http://cuijiahua.com/blog/2018/01/basis_46.html "悬停显示")

|                  Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|      从尾到头打印链表                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_1.md) | |
|      链表中环的入口结点                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_2.md) | |
|      删除链表中重复的结点                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_3.md) | |
|      链表中倒数第k个结点                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_4.md) | |
|      反转链表                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_5.md) | |
|      合并两个排序的链表                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_6.md) | |
|      复杂链表的复制                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_7.md) | |
|      两个链表的第一个公共结点                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_8.md) | |
|      孩子们的游戏                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/LinkedList_9.md) | |


### 递归和循环（Recursion and loop）(4道)：

* [剑指Offer（七）：裴波那契数列](http://cuijiahua.com/blog/2017/11/basis_7.html "悬停显示")
* [剑指Offer（八）：跳台阶](http://cuijiahua.com/blog/2017/11/basis_8.html "悬停显示")
* [剑指Offer（九）：变态跳台阶](http://cuijiahua.com/blog/2017/11/basis_9.html "悬停显示")
* [剑指Offer（十）：矩形覆盖](http://cuijiahua.com/blog/2017/11/basis_10.html "悬停显示")

|                  Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|      斐波那契数列                     | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Loop_1.md) | |
|      跳台阶                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Loop_2.md) | |
|      变态跳台阶                    | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Loop_3.md) | |
|      矩形覆盖                  | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Loop_4.md) | |



### 栈和队列（Stack）(3道)：

* [剑指Offer（五）：用两个栈实现队列](http://cuijiahua.com/blog/2017/11/basis_5.html "悬停显示")
* [剑指Offer（二十）：包含min函数的栈](http://cuijiahua.com/blog/2017/12/basis_20.html "悬停显示")
* [剑指Offer（二十一）：栈的压入、弹出序列](http://cuijiahua.com/blog/2017/12/basis_21.html "悬停显示")

|                  Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|      用两个栈实现队列                     | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Stack_1.md) | |
|      包含min函数的栈                     | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Stack_2.md) | |
|      栈的压入、弹出序列                     | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Stack_3.md) | |

### 时间空间效率的平衡 (4道)：

* [剑指Offer（三十三）：丑数](http://cuijiahua.com/blog/2018/01/basis_33.html "悬停显示")

|                  Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|      丑数                     | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Ugly.md) | |

### 位运算

* [剑指Offer（十一）：二进制中1的个数](http://cuijiahua.com/blog/2017/11/basis_11.html "悬停显示")  
* [剑指Offer（四十八）：不用加减乘除的加法](http://cuijiahua.com/blog/2018/01/basis_48.html "悬停显示")
* [剑指Offer（三十一）：整数中1出现的次数（从1到n整数中1出现的次数）](http://cuijiahua.com/blog/2017/12/basis_31.html "悬停显示")

|                  Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|     二进制中1的个数       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Bit_1.md) | |
|     不用加减乘除的加法       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Add_1.md) | |
|     整数中1出现的次数       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Find_1.md) | |

### 树(15道)：

* [剑指Offer（四）：重建二叉树](http://cuijiahua.com/blog/2017/11/basis_4.html "悬停显示")
* [剑指Offer（十七）：树的子结构](http://cuijiahua.com/blog/2017/12/basis_17.html "悬停显示")
* [剑指Offer（十八）：二叉树的镜像](http://cuijiahua.com/blog/2017/12/basis_18.html "悬停显示")
* [剑指Offer（二十二）：从上往下打印二叉树](http://cuijiahua.com/blog/2017/12/basis_22.html "悬停显示")
* [剑指Offer（二十四）：二叉树中和为某一值的路径](http://cuijiahua.com/blog/2017/12/basis_24.html "悬停显示")
* [剑指Offer（三十八）：二叉树的深度](http://cuijiahua.com/blog/2018/01/basis_38.html "悬停显示")
* [剑指Offer（三十九）：平衡二叉树](http://cuijiahua.com/blog/2018/01/basis_39.html "悬停显示")
* [剑指Offer（五十七）：二叉树的下一个结点](http://cuijiahua.com/blog/2018/01/basis_57.html "悬停显示")
* [剑指Offer（五十八）：对称的二叉树](http://cuijiahua.com/blog/2018/01/basis_58.html "悬停显示")
* [剑指Offer（五十九）：按之字顺序打印二叉树](http://cuijiahua.com/blog/2018/01/basis_59.html "悬停显示")
* [剑指Offer（六十）：把二叉树打印成多行](http://cuijiahua.com/blog/2018/01/basis_60.html "悬停显示")
* [剑指Offer（六十一）：序列化二叉树](http://cuijiahua.com/blog/2018/01/basis_61.html "悬停显示")
* [剑指Offer（二十三）：二叉搜索树的后序遍历序列](http://cuijiahua.com/blog/2017/12/basis_23.html "悬停显示")
* [剑指Offer（二十六）：二叉搜索树与双向链表](http://cuijiahua.com/blog/2017/12/basis_26.html "悬停显示")
* [剑指Offer（六十二）：二叉搜索树的第k个结点](http://cuijiahua.com/blog/2018/01/basis_62.html "悬停显示")

|                 Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|     重建二叉树       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_1.md) | |
|     树的子结构       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_2.md) | |
|     二叉树的镜像       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_3.md) | |
|     从上往下打印二叉树       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_4.md) | |
|     二叉搜索树的后序遍历序列       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_5.md) | |
|     二叉树中和为某一值的路径       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_6.md) | |
|     二叉搜索树与双向链表       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_7.md) | |
|      数据流中的中位数                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_8.md) | |
|      二叉树的下一个结点                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_9.md) | |
|      对称的二叉树                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_10.md) | |
|      按之字顺序打印二叉树                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_11.md) | |
|      把二叉树打印成多行                   | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_12.md) | |
|      二叉搜索树的第k个结点                  | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_13.md) | |
|      序列化二叉树                  | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_14.md) | |
|      二叉树的深度                  | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_15.md) | |
|      平衡二叉树                  | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Tree_16.md) | |


### 其他(15道)：

* [剑指Offer（十二）：数值的整数次方](http://cuijiahua.com/blog/2017/11/basis_12.html "悬停显示")
* [剑指Offer（四十一）：和为S的连续正数序列](http://cuijiahua.com/blog/2018/01/basis_41.html "悬停显示")
* [剑指Offer（四十二）：和为S的两个数字](http://cuijiahua.com/blog/2018/01/basis_42.html "悬停显示")
* [剑指Offer（四十七）：求1+2+3+…+n](http://cuijiahua.com/blog/2018/01/basis_47.html "悬停显示")
* [剑指Offer（六十五）：矩阵中的路径](http://cuijiahua.com/blog/2018/02/basis_65.html "悬停显示")
* [剑指Offer（六十六）：机器人的运动范围](http://cuijiahua.com/blog/2018/02/basis_66.html "悬停显示")

|                 Title                   |                  Python                  |                   C++                    |                   Blog                   |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|     数值的整数次方       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Pow.md) | |
|     和为S的连续正数序列       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/SumS.md) | |
|     和为S的两个数字       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/TwoSumS.md) | |
|     求1+2+3+…+n       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/1nSum.md) | |
|     矩阵中的路径       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Route.md) | |
|     机器人的运动范围       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Robot.md) | |
|     剪绳子       | [Python](https://github.com/Liuhongzhi2018/LeetCode/blob/master/SwordOffer/Cut.md) | |