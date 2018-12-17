#CNNs
CNN
RCNN
MaskRCNN

摘自我的毕设论文：
目前实例分割任务的最好效果，是今年年初由何凯明等学者提出的Mask R-CNN网络结构所取得的[1]，此项工作也获得了2017年ICCV的最佳论文奖。Mask R-CNN是在物体检测网络Faster R-CNN[2]的基础上将ROIPool网络替换成了RoIAlign网络结构（微调bounding box位置以更好适应语义分割的需要），并且在训练时采用了将像素分割和物体检测两个子任务解耦的策略，即针对每个类别估计一个像素分割的二值掩膜，与分类识别和bounding box框选同时进行。原初的R-CNN[4]网络结构是先用选择性搜索（Selective Search）生成大量不同尺寸的候选bounding box(每张正常尺寸的图片大约2k个bounding box)，再由一个预先训练好的AlexNet网络（一种CNN网络）的变体来判别bounding box中是否有物体存在，再通过SVM来对物体进行分类，最后对所有有物体存在的bounding box坐标点做线性回归，聚合成一个最精准的bounding box。而Fast R-CNN[3]则是先用RPN网络结构（Region Proposal Network，也即RoI Pooling）在R-CNN的特征卷积层之上加了一个池化效果，再将经过池化的卷积特征用选择性搜索算法提出候选的bounding box，并进行分类和bounding box回归。这种做法将特征提取过程的效率提高了近两千倍，并将R-CNN的所有操作（CNN特征提取，SVM分类识别，bounding box线性回归）在一个统一的网络框架中实现。而Faster R-CNN则是将R-CNN中用于提出bounding box候选的选择性搜索算法替换成了一层在卷积层之后的全卷积网络，利用卷积层提取的信息来高效地提出bounding box候选（proposal）。以上提到的具体的网络结构（及其演变过程）可见五篇参考文献[1,2,3,4,5]。
