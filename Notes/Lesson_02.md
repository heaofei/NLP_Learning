[toc]

##  实现图的广度优先搜索（BFS）

给定图G（Graph）的起始定点s（start），广度优先搜索通过探索图中的边以找到G中的所有顶点，其中存在从s开始的路径，。通过广度优先搜索，会找到所有与s直接相邻的相距 $k_i$ 的顶点，然后在以这些 $k_i$ 顶点为节点，可以找到直接相邻的距离 $p_i$ 的顶点。其原理可以参考二叉树的BFS遍历过程。

为了跟踪遍历的进度，BFS将每个顶点着色为白色，灰色，或者黑色。在为遍历访问时，所有的顶点初始化为白色。当一个节点最初被发现时，将他置为灰色，当BFS完全探索完一个节点时，将他置为黑色。这意味着一旦节点变为黑色，就再没有与他相邻的白色节点了。另一方面，灰色节点可能还有一些白色的节点与之相邻，仍需要继续的探索。
