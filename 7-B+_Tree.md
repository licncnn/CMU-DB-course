# B+ 树

一般用在表的索引上。  table Index

DBMS 使用一些特定的数据结构来存储信息：

- Internal Meta-data
- Core Data Storage
- Temporary Data Structures
- Table Indexes

本节将介绍存储 table index 最常用的树形数据结构：B+ Tree，Skip Lists，Radix Tree



# Table Index

table index 为提供 DBMS 数据查询的快速索引，它本身存储着某表某列排序后的数据，并包含指向相应 tuple 的指针。DBMS 需要保证表信息与索引信息在逻辑上保持同步。用户可以在 DBMS 中为任意表建立多个索引，DBMS 负责选择最优的索引提升查询效率。但索引自身需要占用存储空间，因此在索引数量与索引存储、维护成本之间存在权衡

存储开销    Storage Overhead

维护开销     MainTenance Overhead





## B+ Tree

B+ Tree 是一种自平衡树，它将数据有序地存储，且在 search、sequential access、insertions 以及 deletions 操作的复杂度上都满足 O(logn)，其中 sequential access 的最终复杂度还与所需数据总量有关。









<img src="C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220508224213185.png" alt="image-20220508224213185" style="zoom:33%;" />























