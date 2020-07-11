# Python
很多人第一次安装的python都是在Python的官网下载的。  
其实，最佳的形式是使用Anaconda来安装python。  

****
这里很多人都会产生疑问。  
不在官网？？  
你这不是在逗我玩吗？？  

Anaconda其实是python的一个包管理器。  
通过Anaconda的**python虚拟环境**，我们可以非常方便的为我们切换python的版本和安装一些复杂的python包（例如[tensorflow](https://www.tensorflow.org/)、[pandas](https://pandas.pydata.org/)、[numpy](https://numpy.org/)、[scrapy](https://scrapy.org/)）。    
上面提到的python包，我相信很多人在安装它们的时候，都被虐得不要不要的。  
在使用了虚拟环境后，这些问题都不会是问题了。
## 虚拟环境  
我不会用很生涩难懂的文字来描述**虚拟环境是什么**？
所以，我用几个实际的示例来说明**为什么我们要使用虚拟环境**？  

### python2.7、python3.5 与 python3.6  
今天，我们接手了三个项目，分别是用python2.7、python3.5 与 python3.6编写的。  
如果我们想要运行这些项目。  
我们需要分别去下载python2.7、python3.5 与 python3.6 的安装包。  
并且要设定它们的环境变量为：  
```bash
python

python3.5

python3.6
```
还要去设定pip的环境变量：  
```bash
pip

pip3.5

pip3.6
```
上面这些操作，在我的新手期。  
我是设定过的。  
可以说超麻烦，而且非常容易发生错误。   
### django 1.11 和 Django2
假设，现在需要我们用python3.6 同时运行分别用**Django1.11**和**Django2**写的两个项目。  
在没有虚拟环境的情况下。  
我可以明确的告诉你，是没有办法同时运行它们。  
会出现包引用失败和路由命名空间的报错。  

### 第三方包集体降级或升级
某些时候，由于包的版本不兼用。  
直接执行`pip install xxxx`  
有一定概率会出现一系列第三方包出现**集体降级或升级**。  
导致一部分之前写好的项目无法运行（概率很小，但是我遇到过）。  
