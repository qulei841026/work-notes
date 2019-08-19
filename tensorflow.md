#TensorFlow

##学习网站
[TensorFlow](https://tensorflow.google.cn){:target="_blank"}<br>
[机器学习](https://developers.google.cn/machine-learning/crash-course/){:target="_blank"}

##Mac安装
```
$ pip install --upgrade tensorflow      # for Python 2.7<br>
$ pip3 install --upgrade tensorflow     # for Python 3.n
```
##MNIST
 深度学习的数据集

##机器学习
###训练集和测试集
测试集不能用去训练，会影响验证的准确性。
###特征
传统编程的关注点是代码。在机器学习项目中，关注点变成了特征表示。

###拟合和泛化

###特征工程
+ 缩放特征值
+ 分箱：特征值划分区间
+ 清理

####特征组合
多个特征值的并集

###神经网络
####Embedding层
[概念](https://blog.csdn.net/weixin_42078618/article/details/82999906)

###相关问题
####问题一: TensorFlow binary was not compiled to use: AVX2 FMA

&emsp;Mac环境下重新编译Tensorflow源码并集成

+ 安装bazel工具: [教程](https://docs.bazel.build/versions/master/install-os-x.html)
    + Mac版本10.14.5下使用bazel-0.26.0版本编译tensorflow-2.0版本。因为低版本bazel无法在Mac-10.14.5系统上工作，所以tensorflow也不能编译低版本。
    + 教程中独立安装第三部执行.sh文件更改为:
    ```
    sudo ./bazel-<version>-installer-darwin-x86_64.sh --user
    ```

+ 编译Tensorflow源码: [教程](https://blog.csdn.net/yhily2008/article/details/79967118)
    + 编译时间太长 

####问题二：futurewarning: passing (type, 1) or '1type' as a synonym of type is deprecat in a future version of numpy
&emsp;numpy使用1.17.0版本导致的，使用Pychram修改numpy版本1.16.0即可解决。


