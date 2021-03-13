# 测例 speacial judge 说明如下：

## chapter2

* ch2_exit: 没有输出就算正确。

## chapter3

第三章测试涉及调度，如果一起运行，不同行的输出可能交错出现。

如果要单独测试，需要调整编译脚本，可以@zyr。

* ch3_0_sleep: `get_time OK! 28` 中 28 只要是正整数就算对。
* ch3_0_sleep1: `delta = 104ms!` 中 104 应该在区间 [80, 120] 内。
* ch3_1_yield[012]: 必须一起运行
* ch3_2_stride[012345]: 优先级与 exit_code 需要基本成正比，误差在 +-10% 内。
* ch3t_deadlock: 无输出，程序在 10s 内结束就算过。

# chapter4

* ch4_mmap1: 没有输出就算过。错误输出见 .fail。
* ch4_mmap2: 没有输出就算过。错误输出见 .fail。

# chapter5

* ch5_spawn0: `new child i` 和 `Test getpid OK! pid = i` 交替出现。只要没种的 `i` 遍历 [k, k+39] 这 40 个数字即可。k 不确定，为正整数。
* ch5_spawn1: `new child i` i 为正整数即可。
* ch5_getpid: `Test getpid OK! pid = i` i 为正整数即可。

# chapter6

QAQ，555555~，我偷的代码出现了迷之bug，调试一晚无果。带 .guess 后缀的是人脑模拟结果。真是输出您可以求助 @小源，这个测例是他出的。

