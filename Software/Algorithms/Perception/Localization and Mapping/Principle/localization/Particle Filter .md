# Particle Filter (粒子滤波)
这是Map Registration地图配准的最常用算法。基于采样和概率模型。先随机采样一些在均值附近的位姿，然后跟踪这些点随里程计的运动过程，在跟踪过程中进行优化、过滤，得出最可能的位姿。详情可参考这篇博客园的[博客](http://www.cnblogs.com/sanmenyi/p/7091978.html)