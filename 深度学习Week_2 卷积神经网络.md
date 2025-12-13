# 深度学习Week_2 卷积神经网络

## 卷积神经网络的应用

常见领域：人脸识别、辅助诊断遗传病、表情识别、图像生成、图像风格转化、自动驾驶

### 分类

对汽车品牌型号进行分类

![屏幕截图 2025-12-11 164426](https://raw.githubusercontent.com/arthur-lee-1/zxj_typora/main/img/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-12-11%20164426.png)

### 检索

给定图片，根据数据库内容进行归类

![屏幕截图 2025-12-11 164442](https://raw.githubusercontent.com/arthur-lee-1/zxj_typora/main/img/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-12-11%20164442.png)

### 检测

框选目标内容

![屏幕截图 2025-12-11 164449](https://raw.githubusercontent.com/arthur-lee-1/zxj_typora/main/img/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-12-11%20164449.png)

### 分割

可看作像素级别的检测

![屏幕截图 2025-12-11 164510](https://raw.githubusercontent.com/arthur-lee-1/zxj_typora/main/img/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-12-11%20164510.png)





## 传统神经网络vs卷积神经网络

传统：参数太多，容易过拟合

卷积：局部关联，参数共享

### 深度学习三部曲

#### Step 1. 搭建神经网络结构

#### Step 2.  找到一个合适的损失函数

交叉熵损失，均方误差，……

#### Step 3. 找到一个合适的优化函数，更新参数

反向传播（BP），随机梯度下降，……



## 卷积神经网络的组成

### 卷积

* 卷积是对两个实变（实数自变量）函数的一种数学操作。

* 在图像处理中，图像以二维矩阵形式输入神经网络，因此需要二维卷积。

![image-20251211171403891](https://raw.githubusercontent.com/arthur-lee-1/zxj_typora/main/img/image-20251211171403891.png)



### 池化

* 保留主要特征的同时减少参数和计算量，防止过拟合，提高模型泛化能力。

* 一般处于卷积层和卷积层之间，全连接层和全连接层之间。

![image-20251211172659324](https://raw.githubusercontent.com/arthur-lee-1/zxj_typora/main/img/image-20251211172659324.png)



### 全连接

* 两层之间的所有神经元都要权重链接。

* 通常全连接层在卷积神经网络尾部。

* 全连接层参数两通常最大。
