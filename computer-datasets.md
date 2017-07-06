## Image datasets
#### MNIST

​        深度学习领域的“Hello World!”！MNIST是一个**手写数字数据集**，它有60000个训练样本集和10000个测试样本集，每个样本图像的宽高为28*28。需要注意的是，此数据集是以二进制存储的，不能直接以图像格式查看。 
​        最早的深度卷积网络LeNet便是针对此数据集的，当前主流深度学习框架几乎无一例外将MNIST数据集的处理作为介绍及入门第一教程。 

#### CIFAR

CIFAR-10包含10个类别，50,000个训练图像，彩色图像大小：32x32，10,000个测试图像。CIFAR-100与CIFAR-10类似，包含100个类，每类有600张图片，其中500张用于训练，100张用于测试；这100个类分组成20个超类。图像类别均有明确标注。CIFAR对于图像分类算法测试来说是一个非常不错的中小规模数据集。 

#### PASCAL VOC

PASCAL VOC挑战赛是视觉对象的分类识别和检测的一个基准测试，提供了检测算法和学习性能的标准图像注释数据集和标准的评估系统。PASCAL VOC图片集包括20个目录：人类；动物（鸟、猫、牛、狗、马、羊）；交通工具（飞机、自行车、船、公共汽车、小轿车、摩托车、火车）；室内（瓶子、椅子、餐桌、盆栽植物、沙发、电视）。PASCAL VOC挑战赛在2012年后便不再举办，但其数据集图像质量好，标注完备，非常适合用来测试算法性能。 

#### MS-COCO

COCO数据集由微软赞助，其对于图像的标注信息不仅有类别、位置信息，还有对图像的语义文本描述，COCO数据集的开源使得近两三年来图像分割语义理解取得了巨大的进展，也几乎成为了图像语义理解算法性能评价的“标准”数据集。Google的开源show and tell生成模型就是在此数据集上[测试](http://lib.csdn.net/base/softwaretest)的。 
目前包含的比赛项目有： 
1.目标检测（COCO Detection Challenge），包含两项比赛：

- 输出目标物的边框即可（using bounding box output），也就是我们常说的目标检测(object detection)了
- 要求把目标物从图像中分割出来（object segmentation output），即我们所说的图像语义分割（Semantic image segmentation）

2.图像标注（COCO Captioning Challenge） 
具体说来就是一句话准确描述图片上的信息（producing image captions that are informative and accurate）。那这个怎么评分呢？目前是靠人工评分。 

3.人体关键点检测（COCO Keypoint Challenge） 
比赛要求是找到人在哪，然后定位到人体的一些关键点位置（The keypoint challenge involves simultaneously detecting people and localizing their keypoints）。

#### ImageNet

Imagenet数据集是目前[深度学习](http://lib.csdn.net/base/deeplearning)图像领域应用得非常多的一个数据集，关于图像分类、定位、检测等研究工作大多基于此数据集展开。Imagenet数据集有1400多万幅图片，涵盖2万多个类别；其中有超过百万的图片有明确的类别标注和图像中物体位置的标注。Imagenet数据集文档详细，有专门的团队维护，使用非常方便，在[计算机视觉](http://lib.csdn.net/base/computervison)领域研究论文中应用非常广，几乎成为了目前深度学习图像领域[算法](http://lib.csdn.net/base/datastructure)性能检验的“标准”数据集。与Imagenet数据集对应的有一个享誉全球的“ImageNet国际计算机视觉挑战赛(ILSVRC)”，目前包含的比赛项目有： 

1.目标定位（Object localization） 
给定一幅图像，算法需要生成5个带有置信度的类别标签及其分别对应的目标物边框信息。算法准确率的评估是基于与标注的类别标签最匹配的预测标签图片中可能存在多个物体及其对应的标注信息和与标注的边框信息重叠的预测边框图片中可能存在多个同类物体。为什么这样做呢？因为这样就允许算法识别图像中的多个目标物，并且当其中一个目标物确实存在于图像中但没有被标注出来时算法不会受到惩罚。可能说的有不清楚或不正确的地方，大家可以看下[官方的评估规则](http://image-net.org/challenges/LSVRC/2016/index#loc)。 
2.目标检测（Object detection） 
给定一幅图像，算法需要生成多组(ci,si,bi)形式的预测信息，其中ci为类别标签、si为置信度、bi为边框信息。需要注意的是，算法必须检测出图像中出现的每一个训练过的目标物，漏检和重复检测都会受到惩罚。 
3.视频序列的目标检测（Object detection from video） 
这一项和上一项目标检测类似。 
4.场景分类（Scene classification） 
这个比赛使用了[Places2 dataset](http://places2.csail.mit.edu/)，比赛规则是对于给定图像，允许算法产生5个场景分类，并挑选匹配度最高的作为评估结果，详看他们的评估规则吧。为什么这么做呢？因为同一幅图片可以包含有多个场景类别，事实上同一幅图片本来就是用多个类别标注的。 
5.场景分析（Scene parsing） 
这个比赛的目标是将图像分割成与语义类别相关联的不同图像区域，如天空，道路，人和床。

#### OpenImage
https://github.com/openimages/dataset

## Face datasets
#### AFLW
#### FDDB
#### LFW
#### CelebA
#### EmotioNet

## Video datasets
#### Youtobe-8M
#### Kinetics
Kinetics视频数据集由 DeepMind发布，是高质量的大型 YouTube 视频URL数据集，涵盖多种多样的人类行为，其目的是帮助机器学习社区提升其模型对于视频的理解。该数据集大约包含300,000个视频片段，包含400个人类行为类别，每个类别至少包含400个视频片段，每个视频片段大约10秒，并标注一个单一类别。
下载地址：https://deepmind.com/research/open-source/open-source-datasets/kinetics/

#### Something-something
Something-something数据集包含 108,499 个标注视频片段，它们每一个的时长都在2 到 6 秒之间。这些视频展示了 175 种类别的物体和动作。这些文字题注（captions）都是基于模版的文字描述，比如“把某物丢进某物”这种文字模板。模板往往包含“某物”的“窄条”（slots），就像物体的占位符号（placeholders）。这就给网络中从文本到视频的编码过程（text-to-video encoding）提供了附加结构，从而来增强学习效果。
此数据集的目的不仅仅是在视频中检测和追踪物体，而且还是为了破译人类行为者（human actors）的表现和那些直接或间接地操作物体的动作。根据视频来预测文本标注往往需要强视觉特征（strong visual features），这些特征能够表征物体和这个世界中的大量物理特性。这就包括那些属性的相关信息，比如空间关系和材料属性。
下载地址：https://www.twentybn.com/datasets/something-something

#### Jester
Jester数据集包括 148,092 个标注视频片段，每一个时长 3 秒左右。这些视频涵盖了 25 个类别的人类手势和两个“无手势”的类别，从而来帮助网络结构对特定手势动作和未知手部动作进行区分。这些视频展示了人类行为者在网络摄像机面前完成各种一般的手势的过程，比如“向左或向右重击”，“两个手指向上或向下滑动”，“向前或向后摆手”。从视频中预测这些文本标注通常要求网络能够理解这些概念，比如三维空间的自由度（震荡、摇摆、举起等等）。
传统的手势识别系统往往需要像立体相机或深度传感器这样的特殊硬件，比如时差测距相机（time-of-flight cameras）。我们能够使用 Jester 数据集训练一个神经网络，它可以根据原始的三原色（RGB）输入对所有的 25 种手势进行检测和分类，测试精度可达 82%。此系统可在大量的嵌入式平台上进行实时运行，这些平台都使用网络摄像机进行视频输入。
下载地址：https://www.twentybn.com/datasets/jester

## QA datasets
#### MS MARCO






## Self-Driving-Car datasets
#### KITTI

KITTI由德国卡尔斯鲁厄理工学院(Karlsruhe Institute of Technology)和丰田芝加哥技术研究院(Toyota Technological Institute at Chicago)于2012年联合创办，是目前国际上最大的**自动驾驶场景下的计算机视觉算法评测数据集**。用于评测3D 目标（机动车、非机动车、行人等）检测、3D 目标跟踪、道路分割等计算机视觉技术在车载环境下的性能。KITTI包含市区、乡村和高速公路等场景采集的真实图像数据，每张图像中多达15辆车和30个行人，还有各种程度的遮挡。

#### CitySpace

Cityscapes也是自动驾驶相关方面的数据集，重点关注于**像素级的场景分割和实例标注**。 

下载地址： https://www.cityscapes-dataset.com

####  Tusimple Benchmark

TuSimple Benchmark是图森未来专门为自动驾驶算法研发测试打造的专用数据集。该数据集包括大量时长1秒钟的视频，均遵奉真实路况。相比于传统CV数据集，图森最新发布的这套数据集更加注重实用性，将很多智能驾驶当中的实际问题考虑了进来。TuSimple Benchmark 包含两个子任务为**车道线检测**和**速度估算**。

下载地址：**http://benchmark.tusimple.ai/**

## Age-gender datasets
#### Adience

## Flower
## Pedestrian

## ADE20K



PS： 
数据集组织方式：   [免费/注册/申请/收费]

1. 数据集基本简介
2. 常见的标注(比赛项目)
3. 数据集大小：训练集/测试集合大小
4. 下载地址

TBD：

整理好分类目录

1. 医疗

2. 农业

3. 场景

4. 分类

5. 人体(姿势/人脸/表情)

   ​