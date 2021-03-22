### 1. Hog 是基于灰度直方图的一个检测，具体来说：  
··· 通俗的讲：

HOG特征提取方法就是将一个image：

1.            灰度化（将图像看做一个x,y,z（灰度）的三维图像）

2.            划分成小cells（2*2）

3.            计算每个cell中每个pixel的gradient（即orientation）

4.            统计每个cell的梯度直方图（不同梯度的个数），即可形成每个cell的descriptor
————————————————
原文链接：https://blog.csdn.net/abcjennifer/article/details/7365651···

### 2. RCNN:  
if the training data is limited, we can use a pre-trained data model plus a specific data we have for the refinement.  
detail [link](https://zhuanlan.zhihu.com/p/158218471)  
``` RCNN包含了三个主要的模块：

生成类别独立的regoin proposal（区域建议），为感知器定义候选区域
CNN提取固定长度的特征
线性SVM分类器进行类别的分类 ```  

