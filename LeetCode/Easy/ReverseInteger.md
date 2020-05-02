
# ReverseInteger

## 问题分析
给定一个范围为 32 位 int 的整数，将其颠倒。
注意:
假设我们的环境只能处理 32 位 int 范围内的整数。根据这个假设，如果颠倒后的结果超过这个范围，则返回 0。

## 编程实现
``` C
int reverse(int x) {
    int i;
    int n = 0;
    if (x < 0) {
	printf("-");
        i = 0 - x;
	}
	do {
           printf("%d", i % 10);
           n++;
           if (n>32) break;
	} while ((i /= 10) != 0);

     if (n <= 32) return i;
     else return 0;
}
```

## 总结体会
整数颠倒输出时，需要考虑各个数位上值的变化。除从个位向高位输出的方法外，还可以考虑使用字符数组输出。