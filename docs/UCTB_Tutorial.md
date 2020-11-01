# UCTB Tutorial

UCTB repository:  https://github.com/uctb/UCTB/ 

UCTB document: https://uctb.github.io/UCTB/ 

这是一份为在UCTB小组实习的同学们编写的简单介绍文档，用于补充主页上没有的一些知识，也作为快速了解我们整个项目的小教程。

## Quick Start

快速上手前，可以先了解以下知识：

* **GCN**：图卷积网络，可以参考下面这篇综述（有好的资源可以补充~）

  Wu, Z., Pan, S., Chen, F., Long, G., Zhang, C., & Yu, P. S. (2019). A Comprehensive Survey on Graph Neural Networks. ArXiv:1901.00596 [Cs, Stat]. http://arxiv.org/abs/1901.00596

* 频域GNN ChebNet: https://zhuanlan.zhihu.com/p/106687580 

* **attention 机制**：可以参考的资料比较多，自行搜索一下~

**实习的任务一般是基于UCTB工具箱，实现一些新的特性**，新特性可以参考我们的[future work]( https://docs.qq.com/doc/DTlJDaXFCTmJlR2tp )界面。完成实习任务，可以按照下述步骤进行：

**Step 1**: 熟悉STMeta模型

​	STMeta的论文可以从此处[下载](http://47.94.208.154/STMeta.pdf )，需要看懂论文。另外论文麻烦不要外传~

**Step 2**: 安装UCTB工具箱

​	UCTB是基于tensorflow的，推荐环境如下：

```python
tensorflow==1.13.1   # 推荐安装GPU版本
python==3.6.5 +  # Python版本也不要太高
```

​	配置好python等环境后，需要安装UCTB工具箱，UCTB的工具箱可以从上面的repository的链接[下载](https://github.com/uctb/UCTB/ )，下载好工具箱后，进入UCTB根目录，执行安装指令：

```pythotn
python build_install.py
```

​	至此，UCTB的工具箱就安装好啦，如果有什么问题，检查一下依赖是否已安装和python的版本，如果还有问题，可以一起讨论一下~

**Step 3**: 熟悉STMeta的实现以及实验的运行方法

​	安装好工具箱后，我们就可以对照着STMeta的论文查看UCTB中STMeta模型的实现了，STMeta的模型在

`\UCTB\UCTB\model\STMeta.py`中。

​	在熟悉了STMeta的实现后，我们还需要介绍我们的实验的运行方法，通常实验的运行代码在`\UCTB\Experiments\`目录下。我们进入Experiment目录下的STMeta子目录，这是我们STMeta模型的运行代码存放的目录。由于版本的多次更新，目前最新的运行文件是`RunnerKDD.py`

​	很显然，要运行一个实验，我们需要给模型喂入数据集（给出地铁上海的数据集作为demo [下载](http://47.94.208.154/Metro_Shanghai.zip)，如果有其他数据集需求的，可以找我要~）。除了数据集，我们还需要指定一些超参数，我们以`RunnerKDD.py`中的内容为例，简单介绍一些参数的含义:

```python
os.system('python STMeta_Obj.py -m STMeta_v1.model.yml -d metro_shanghai.data.yml '
          '-p graph:Distance-Correlation-Line,MergeIndex:3')
```

​	上述代码是运行STMeta_V1模型的代码，关于V1的具体含义，可以参考[此处]( https://uctb.github.io/UCTB/md_file/all_results.html )。我们可以看到，在运行的时候，我们为STMeta模型指定了模型参数文件`STMeta_v1.model.yml`和数据参数文件`metro_shanghai.data.yml`。模型参数文件里面保存着模型的超参数（例如LSTM hidden size是多少），数据参数文件指定了我们读取数据的一些参数（例如一些构建图的阈值，是否normalization等）。除了上述两个参数之外的，还有以`-p`开头的一系列更新参数，例如`graph`（使用空间图的类型）和`MergeIndex`（控制数据粒度的参数，例如原始数据是5mins，指定MergeIndex为3后，数据的粒度就变为15mins了）。

​	最终运行的方式也十分简单，在shell中执行：

```python
python RunnerKDD.py
```

## 数据集的存放

在下载了数据集后，直接解压到`UCTB/Experiment/STMeta`目录下是无效的，原因是UCTB只会从安装的package中寻找数据文件，我们需要手动将数据集文件放入UCTB package中的`data`子目录下，以我的机器为例，我的UCTB python package路径如下：

```
C:\Users\81512\AppData\Local\Programs\Python\Python36\Lib\site-packages\UCTB
```

我需要将`Metro_Shanghai.pkl`放入上述路径下的`data`子目录下。

## 数据集的格式

以下为UCTB的数据集的通用格式，数据使用pickle库进行读写。可以看出dict_keys为：(['TimeRange', 'TimeFitness', 'Node', 'Grid', 'ExternalFeature'])，流量数据储存在"Node"中的"TrafficNode"或者"Grid"中的"TrafficGrid"中。（如果感兴趣的话，可以参考Metro_Shanghai.pkl文件观察一下）

```python
DataFormat = {
    "TimeRange": [],    # 起止时间 str eg:['2016-10-01', '2016-11-30']
    "TimeFitness": [],  # 时间粒度 int 单位为min
    "Node": {
        "TrafficNode": [],  # with shape [time_slots, num-of-node] eg:(1440,256) 
        "TrafficMonthlyInteraction": [],
        "StationInfo": [],  # list eg:['0', 0, 34.210542575000005, 108.91390095, 'grid_0']
        "POI": []
    },
    "Grid": {
        "TrafficGrid": [], # with shape [slots, num-of-node. num-of-node] eg:(120, 256, 256)
        "GridLatLng": [],  # 对角线点的经纬度 eg:[[34.20829427, 108.91118]]
        "POI": []
    },
    "ExternalFeature": {
        "Weather": []
    }
}
```

