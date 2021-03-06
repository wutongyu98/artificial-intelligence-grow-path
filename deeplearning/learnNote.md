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
``` 
RCNN包含了三个主要的模块：
生成类别独立的regoin proposal（区域建议），为感知器定义候选区域
CNN提取固定长度的特征
线性SVM分类器进行类别的分类 
```  

### 3. Mask_RCNN TensorFlow版本安装和应用实战[link](https://blog.csdn.net/qiancaobaicheng/article/details/95521456)只能在TensorFlow1.x版本运行，需要在conda环境中配置 
#### 3.1 在conda中添加科大源版本方法
```
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/msys2/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/bioconda/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/menpo/

conda config --set show_channel_urls yes``
原文链接：https://blog.csdn.net/weixin_41955987/article/details/107170352
```
#### 3.2 用conda和科大镜像安装cuda  
conda install cudatoolkit=8.0   

#### 3.3 keras 降级处理和  
pip uninstall keras  
pip install  keras==2.0.8  
#### 3.4 TensorFlow和keras的对应关系[link])(https://blog.csdn.net/qq_37171215/article/details/108567516)  
#### 3.5 conda 安装TensorFlow  
```
conda search tensorflow-gpu     //查找现有版本
conda install tensorflow-gpu==1.5.0   
```
### 4. 这次的MaskRCNN的TensorFlow版本调试持续两整天，终于告一段落。主要问题市TensorFlow， keras, numpy, cuda, cudnn 版本的协调，正确的版本配置为：  
```
conda install cudatoolkit=8.0
pip install keras==2.1.6
numpy 1.6
conda install cudnn=7.0.5
```
