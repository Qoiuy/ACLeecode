# 思路及结题步骤

###### Diameter of Binary Tree

###### 求二叉树直径

前两天公司开发爬虫。+陷入了遍历的死循环。


###### 那天的想法是 ：求直径 就得求，对于每一个节点都需要求一遍。不然可能会出问题。
今天又看了看。发现。可以将二叉树伸直到一个list里面。
而单纯求直径的话。不需要放list里面。只需记忆当前点即可。
。。。还是用list吧。。使用list然后直接返回list的长度即可。

###### 解题思路
使用linkedlist addFirst removeFirst addLast removeLast
1.找到最左节点。
2 tmp节点存放最左节点的父节点 length存放最左节点到父节点的路径。
3 判断tmp节点的右节点， 长度是否有长与左节点长度的。如果有 替换最左节点。 为右节点。


###### 思路错误：
按照我的方式，，无法找到最左节点。
https://kingsfish.github.io/2017/07/13/Leetcode-543-Diameter-of-Binary-Tree/
此人思路很厉害

###### 遍历一遍 返回节点左子树和右子树的深度。

1求当前节点的深度。
