## rCore_tutorial_v3 TESTS

更新通知：make 命令经过优化，使用格式改为　`make all CHAPTER=x` 可获得第 x 章的测例。

* 可选项 2，3_0, 3_1, 3_2，4, 5, 6, 7。

**重要**-加载地址更新： 
  * chapter2 所有程序加载位置位于 0x80400000，与示例代码一致。
  * chapter3 测试程序分为3批，每一批的地址都为 0x80400000 + id*0x20000，id 为程序在这一批中的序号。每一批都与参考代码一致，请分别测试。
  * chapter4-7 所有程序加载位置位于 0x0，与示例代码一致。

可以在 `user/build/asm` 目录下查看汇编来确认加载地址。

其他内容详见 [guide](./guide.md) 。

