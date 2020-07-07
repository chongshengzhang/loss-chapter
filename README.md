# loss-chapter
**This project is the sharing of code of experiments in loss chapter of DL book.**
## Requriment
This is my experiment enviroument,you can make a change according to your hardware.<br/>
* Linux Mint 19.1
* python 3.7.7
* pytorch-cpu 1.1.0
* tensorboardX 1.7

<<<<<<< HEAD
## Introduction
File "losses" contains loss functions can be used in exp2,exp3 and exp4.You must copy them to the your working file<br/>
File "exp1","exp2","exp3" and "exp4" include main code of each experiment.<br/>
"Exp4" is loss functions comparison experiment."1" is vgg model and "2" is EfficientNet model.<br/>
I add _all_lost.py_ including all lost function we may used in all project.You can have a look at functions and use them.Make sure you also have two other losses.

#### Dataset
| _experiment_ | exp1 | exp2 | exp3 | exp4|
| :------:| :---:| :---:| :---:| :---: |
| _dataset_| toy data included in code| [MNIST](http://yann.lecun.com/exdb/mnist/)| build it yourself| [CIFAR100](https://www.cs.toronto.edu/~kriz/cifar.html)|
You can make your own dataset in exp3,pay attention to the ratio of two catagories.<br/>
You can download MNIST and CIFAR through torchversion.datasets,we have set _download_ = _True_ in exp2.<br/>
If something wrong happens,you can download by clicking the links above.

#### Model
| _experiment_ | exp1 | exp2 | exp3 | exp4|
| :------:| :---:| :---:| :---:| :---: |
| _model_| toy regression | LeNet++ | LeNet | Vgg16 <br/> EfficientNet |
  
#### Reference
This project absorded essences of other project on github and other websites.<br/>
Source of part exp2 is miss.<br/>

| _ours_ | losses\center_loss.py | losses\Focalloss.py | exp1\train.py | exp4 | EfficientNet-b0 model
| :-----:| :----:| :----:| :----:| :----:| :----:|
| _source_ | [KaiyangZhou](https://github.com/KaiyangZhou/pytorch-center-loss/blob/master/center_loss.py) | [Kingslayer_](https://blog.csdn.net/qq_33278884/article/details/91572173)|[SherlockLiao](https://www.jianshu.com/p/331a995774d8)|[weiaicunzai](https://github.com/weiaicunzai/pytorch-cifar100)|[Rwightman](https://github.com/rwightman/gen-efficientnet-pytorch)

## Usage
All experiments follow deep learning pipeline: 
* data load and preprocess
* model build or load
* loss function ,parameters and optimizer set 
* run model and get results<br/>
<br/>
* For exp1,you can run directly.If you want to see the result of one particular loss ,you can make other losses invisible by "#" at visulization part.
* For exp2 exp3 and exp4,some mecessary files like _"data"_ can be made by programes.You must download dataset and put them on right dictionary assigned by programs.
* For different losses comparasion in different experiments,you can copy the code file and tune hyperparameters and change loss functions.
* In exp2,_gif_generatory.py_ can help you to generate gif.You must input the path of your first epoch picture.
* In exp4,_trainmail.py_ is a python program can send mail about train,you must set variales in the program.<br/>

##
_There maybe something incorrect unrealized before,I will be grateful if you can point out._

__Copyright: This work was designed by Prof. Chongsheng Zhang (chongsheng.zhang@yahoo.com)<br/>And implemented by Mr. Dazheng Liu (liudz@henu.edu.cn), a master student of Henan University under the supervision of Prof. Zhang.__<br/>
__This software is free for academic use only. For commercial companies, you should first ask the permission from both authors above.__ 


=======
## 文件介绍与注意
* 实验序号为本章节中对应实验序号，实验四即损失函数对比实验。center loss参考[这里](https://github.com/KaiyangZhou/pytorch-center-loss/blob/master/center_loss.py),
focal loss参考[这里](https://blog.csdn.net/qq_33278884/article/details/91572173)。<br/>
* losses文件夹中的损失函数可用于实验二三四中，需将其放在对应文件夹下。<br>
* 实验二所用数据MNIST可由程序自动下载，或者到[官网](http://yann.lecun.com/exdb/mnist/)下载，实验四使用CIFAR100可以在[官网](https://www.cs.toronto.edu/~kriz/cifar.html)下载。<br/>
* 实验一参考[这里](https://www.jianshu.com/p/331a995774d8)，每次运行结果略有不同但总体符合趋势，可单独打印显示损失变化趋势。<br/>
* 实验二参考代码与特征打印代码参考自网络，出处遗失。提供程序使用交叉熵优化，使用center loss可将文件重新保存更改损失，并打印出每个批次的特征图像，gif_generator.py可将一组图像生成动态图。<br/>
* 实验三与实验二代码基本相同，我们选用了LeNet网络，训练数据需要自己亲手设计，尽量使两类数据比例尽可能大。<br/>
* 实验四主要代码参考[这里](https://www.cs.toronto.edu/~kriz/cifar.html)并做出适应性改变，其中1中包含trainmail可以在一定epoch后发送到指定电子邮箱，但需要进行设置，EfficientNet所用模型来自[这里](https://github.com/rwightman/gen-efficientnet-pytorch)。<br/>

_写作、整理仓促，难免有不恰当之处，欢迎交流！_
>>>>>>> 6ab631b6819f9e594807858ba3c126ba1101a74f
