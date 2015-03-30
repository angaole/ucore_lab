练习

练习1：实现 first-fit 连续物理内存分配算法（需要编程）
在实现first fit 内存分配算法的回收函数时，要考虑地址连续的空闲块之间的合并操作。提示:在建立空闲页块链表时，需要按照空闲页块起始地址来排序，形成一个有序的链表。可能会修改default_pmm.c中的default_init，default_init_memmap，default_alloc_pages， default_free_pages等相关函数。请仔细查看和理解default_pmm.c中的注释。

请在实验报告中简要说明你的设计实现过程。请回答如下问题：

    你的first fit算法是否有进一步的改进空间


练习2：实现寻找虚拟地址对应的页表项（需要编程）

    请描述页目录项（Pag Director Entry）和页表（Page Table Entry）中每个组成部分的含义和以及对ucore而言的潜在用处。
    如果ucore执行过程中访问内存，出现了页访问异常，请问硬件要做哪些事情？

练习3：释放某虚地址所在的页并取消对应二级页表项的映射（需要编程）

    数据结构Page的全局变量（其实是一个数组）的每一项与页表中的页目录项和页表项有无对应关系？如果有，其对应关系是啥？
    如果希望虚拟地址与物理地址相等，则需要如何修改lab2，完成此事？ 鼓励通过编程来具体完成这个问题
