### 1. Hog 是基于灰度直方图的一个检测，具体来说：  
··· 通俗的讲：

HOG特征提取方法就是将一个image：

1.            灰度化（将图像看做一个x,y,z（灰度）的三维图像）

2.            划分成小cells（2*2）

3.            计算每个cell中每个pixel的gradient（即orientation）

4.            统计每个cell的梯度直方图（不同梯度的个数），即可形成每个cell的descriptor
————————————————
版权声明：本文为CSDN博主「Rachel-Zhang」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/abcjennifer/article/details/7365651···

### 2. if the training data is limited, we can use a pre-trained data model plus a specific data we have for the refinement.  
