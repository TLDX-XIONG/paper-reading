# 深度学习论文阅读
对已经读过的论文和将要读的论文进行梳理，以便自己总结。


## 经典分类网络
| 完成 | 发表时间 | 标题 | 封面 | 贡献 |
| -- | -- | -- | -- | -- |
| ✅ | 2012 |[AlexNet](https://papers.nips.cc/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf)| <img src='Imgs/AlexNet.png' width=200px>  | 深度学习的开篇之作，第一次将深度学习技术引入图像分类中。在ImageNet分类竞赛中远远领先第二名。使用了两块显卡训练，隐式地使用了分组卷积，第一次提出了一些概念(多GPU，分组卷积，最大池化，ReLU，Dropout)，奠定了现代卷积网络的架构。|
| | 2013 |[ZFNet](https://arxiv.org/pdf/1311.2901v3.pdf) | <img src='Imgs/ZFNet.png' width=200px> | 最大的亮点是利用反卷积可视化技术对卷积核可视化，增加了网络的可解释性。 |
| ✅ | 2014 |[VGGNet](https://arxiv.org/pdf/1409.1556.pdf) | <img src='Imgs/VGGNet.png' width=200px> |搭建了一个更深的网络，提出了使用多个小卷积核能够与大卷积核获得相同的感受野，同时能够显著减少参数量。提出了卷积 Block 的概念，通道呈二进制的增加(更能利用计算资源) |
| ✅ | 2014 |[GoogLeNet(Inception V1)](https://arxiv.org/pdf/1409.4842.pdf) | <img src='Imgs/GoogLeNet.png' width=200px> | 提出了在同一层利用多个不同尺度的卷积提取特征，再将得到的特征拼接起来传入下一层作为输入 |
| | 2015 |[Inception V2-V3](https://arxiv.org/pdf/1512.00567.pdf) | <img src='Imgs/InceptionV2-V3.png' width=200px> | |
| | 2016 |[Inception V4](https://arxiv.org/pdf/1602.07261.pdf) | <img src='Imgs/InceptionV4.png' width=200px> |
| ✅ | 2015 |[ResNet](https://arxiv.org/pdf/1512.03385.pdf) | <img src='Imgs/ResNet.png' width=200px> | 提出了残差结构，解决了卷积网络无限堆叠卷积层产生的性能退化问题。使用残差链接能够很好的将深层的 loss 传至浅层，解决了因为链式法则带来的梯度弥散问题。 |
|  | 2016 | [DenseNet](https://arxiv.org/pdf/1608.06993v5.pdf) | <img src='Imgs/DenseNet.png' width=200px> | 在残差连接时，进行通道的 Concatenat 而不是进行简单的相加 |
| | 2017 |[ResNext](https://arxiv.org/pdf/1611.05431.pdf) | <img src='Imgs/ResNext.png' width=200px> | 在 ResNet基础上引入了分组卷积，这样在相同参数量的情况下，ResNext 可以使用更大的通道，获得更多的特征图。 |
| | 2017 | [SENet](https://arxiv.org/abs/1709.01507v4) | <img src='Imgs/SENet.png' width=200px> | 使用了 chanel attention，使其能更加关注感兴趣，有用的通道特征。 |

## 目标检测
| 完成 | 发表时间 | 标题 | 封面 |贡献 |
| -- | -- | -- | -- | -- |
| | 2014 |[R-CNN](https://arxiv.org/pdf/1311.2524v5.pdf) | <img src='Imgs/R-CNN.png' width=200px> | |
| | 2015 |[Fast R-CNN](https://arxiv.org/pdf/1504.08083v2.pdf) | <img src='Imgs/Fast-R-CNN.png' width=200px> | |
| | 2015 |[Faster R-CNN](https://arxiv.org/pdf/1506.01497v3.pdf) | <img src='Imgs/Faster-R-CNN.png' width=200px> |
| | 2016 |[SSD](https://arxiv.org/pdf/1512.02325v5.pdf) | <img src='Imgs/SSD.png' width=200px> |
| ✅ | 2016 |[YOLO](https://arxiv.org/pdf/1506.02640v5.pdf) | <img src='Imgs/YOLOV1.png' width=200px> |
| | 2017 |[Mask R-CNN](https://arxiv.org/pdf/1703.06870v3.pdf) | <img src='Imgs/Mask-R-CNN.png' width=200px> | |
| ✅ | 2017 |[YOLO V2](https://arxiv.org/pdf/1612.08242v1.pdf) | <img src='Imgs/YOLOV2.png' width=200px> |
| ✅ | 2018 |[YOLO V3](https://arxiv.org/pdf/1804.02767v1.pdf) | <img src='Imgs/YOLOV3.png' width=200px> |
| ✅ | 2020 |[YOLO V4](https://arxiv.org/pdf/2004.10934.pdf) | <img src='Imgs/YOLOV4.png' width=200px> |
| | 2018 |[RetianNet](https://arxiv.org/pdf/1708.02002.pdf) | <img src='Imgs/RetainNet.png' width=200px> |

## 语义分割
| 完成 | 发表时间 | 标题 | 封面 |贡献 |
| -- | -- | -- | -- | -- |

## 轻量化网络
| 完成 | 发表时间 | 标题 | 封面 |贡献 |
| -- | -- | -- | -- | -- |
| | | [SqueezeNet]() | <img src='Imgs/SqueezeNet.png' width=200px> | |
| ✅ | | [MobileNet]() | <img src='Imgs/MobileNet.png' width=200px> | |
| ✅ | | [MobileNet V2]() | <img src='Imgs/MobileNet-V2.png' width=200px> | |
| ✅ | | [MobileNet V3]() | <img src='Imgs/MobileNet-V3.png' width=200px> | |
| ✅ | | [ShuffleNet] | | | <img src='Imgs/ShuffleNet.png' width=200px> | 使用了分组卷积和通道 shuffle，减少参数量的同时保证了精度 |
| ✅ | | [ShuffleNet V2]() | <img src='Imgs/ShuffleNet-V2.png' width=200px> | |
| | | [EfficentNet]() | <img src='Imgs/EfficientNet.png' width=200px> | |

## 深度学习使用的 Tricks
| 完成 | 发表时间 | 标题 | 封面 |贡献 |
| -- | -- | -- | -- | -- |
| | 2015 | [Batch Normalization](https://arxiv.org/pdf/1502.03167.pdf) | <img src='Imgs/BN.png' width=200px> | |


## 重识别
| 完成 | 发表时间 | 标题 | 封面 |贡献 |
| -- | -- | -- | -- | -- |

## 其它
| 完成 | 发表时间 | 标题 | 封面 |贡献 |
| -- | -- | -- | -- | -- |
