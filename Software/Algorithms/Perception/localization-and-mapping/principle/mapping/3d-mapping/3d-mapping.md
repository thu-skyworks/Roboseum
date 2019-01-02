# 3D Mapping

当数据维度从2维扩展到3维，Occupancy Grid Mapping 在信息存储上低效的缺点就充分暴露了出来： ![Alt text](../../../../../../../.gitbook/assets/1546192242493.png) 因此Occupancy Grid Map 的数据结构常用于2维地图的构建。

而列表法的表示虽然在信息存储上非常高效，但是搜索起来运算量太大： ![Alt text](../../../../../../../.gitbook/assets/1546192300405.png) 因此在3维中通常使用的是树结构，常用的树结构有两种：[KD树](https://en.wikipedia.org/wiki/K-d_tree)和[八叉树](https://en.wikipedia.org/wiki/Octree)。 ![](../../../../../../../.gitbook/assets/1546192397305.png) ![Alt text](../../../../../../../.gitbook/assets/1546192501079.png)

