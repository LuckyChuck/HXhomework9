# Thinking1	什么是Graph Embedding，都有哪些算法模型 #

答：在互联网场景下，数据对象之间更多呈现的是图结构。典型的场景是由用户行为数据生成的物品全局关系图，以及加入更多属性的物品组成的知识图谱。而在这种情况下，传统的embedding方法已经不能满足了。Graph Embedding是一种针对于图网络的embedding技术。从图网络中进行特征提取。

主要方法：
1.factorization methods （图因式分解机）
2.random walk techniques（随机游走） （课上）
3.deep learning（深度学习）  （课上）


# Thinking2	如何使用Graph Embedding在推荐系统，比如NetFlix 电影推荐，请说明简要的思路 #

答：可以借鉴课上的Deepwalk算法中的那个图例，用电影推荐举例，在基于用户的情况来说，每个人都有看了一些影片，比如说是按照时间维度来说，就在电影之间产生了电影之间的有向边，比如电影A => 电影B =>  电影C
当集合很多用户的数据的时候，这些电影之间就形成了一个有向图，这时，可以利用Graph Embedding的思想对图进行embedding，之后可以利用word2vec等对电影进行计算。产生推荐效果。


# Thinking3	数据探索EDA都有哪些常用的方法和工具 #
1.首先有一些pandas的常用方法，例如：isnull,value_counts,head,shape,info,describe,columns等等
2.有一些常用的分析方法，如pearson系数方法，可以很简洁的看出来各个特征之间的线性关系，可以帮助我们做特征工程。
3.有一些很方便的可视化工具。如missingno，pandas_profiling 等。
