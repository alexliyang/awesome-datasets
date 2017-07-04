## Image datasets
#### MNIST
#### CIFAR
#### PASCAL VOC
#### MS-COCO
#### ImageNet
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
#### CitySpace
下载地址： https://www.cityscapes-dataset.com

## Age-gender datasets
#### Adience

## Flower
## Pedestrian
