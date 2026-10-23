# 注释  
(2026/10/23 15:54:36)

“which aims to localize ground-level query images by matching against a database of aerial images” ([Workman 等, 2015, p. 1](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=1&annotation=CGDRP34G)) CVGL的任务目标

“there are still very large geographic regions with few images” ([Workman 等, 2015, p. 1](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=1&annotation=5FFXNBVH)) 很多区域的地面图像有限，解释为什么要使用航空影像

“cross-view training for learning a joint semantic feature space from different image sources;” ([Workman 等, 2015, p. 1](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=1&annotation=W8BIJSZA)) CVGL实现定位的关键，能够学习不同视角的特征进行匹配

“based on its appearance” ([Workman 等, 2015, p. 2](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=2&annotation=L7MF6I9G))

“The end result of cross-view training is a CNN that is able to extract semantically meaningful features from aerial images without manually specifying semantic labels.” ([Workman 等, 2015, p. 3](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=3&annotation=PATG577N)) 模型训练最终结果，训练的时候需要标签吗？

“cross-view training approach to adapt a network trained for ground-level feature extraction to aerial imagery.” ([Workman 等, 2015, p. 3](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=3&annotation=Z2VCHV4Q)) 如何进行训练，实现跨视角提取特征

“Given a set of ground-level training images, {Ii}, with known location, {li} and known ground-level feature extractor parameters, Θg, we seek a set of parameters, Θa, that minimize the following objective function:” ([Workman 等, 2015, p. 3](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=3&annotation=S9YBMABB)) 训练过程的数学解释

“It is possible that the nearest object in the scene is hundreds of meters away or that the furthest object is tens of meters” ([Workman 等, 2015, p. 3](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=3&annotation=GPRFYXJB)) 地理定位的难点

“Rather than mapping a single ground-level image to a single aerial image, the multi-scale approach allows for a ground-level image to be matched to aerial images at multiple scales.” ([Workman 等, 2015, p. 3](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=3&annotation=QCI4JWJ2)) 多个尺度进行匹配，是指多张图片还是什么？  
**原来的训练是"一张街景照片必须配上它的那一张航拍图"，多尺度改成"一张街景照片可以同时和多张不同缩放级别的航拍图配对"**

“Cross-View USA (CVUSA) dataset” ([Workman 等, 2015, p. 3](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=3&annotation=QR69CAKS))

“the goal is to use a database of aerial images, with known location, to estimate the geographic location of a ground-level query image in that region.” ([Workman 等, 2015, p. 4](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=4&annotation=NBQUJRQ7)) 跨视角地理定位的目标

“because of the dramatic appearance differences between ground-level and aerial viewpoints.” ([Workman 等, 2015, p. 4](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=4&annotation=39N27I28)) 难点

“We directly compare the groundlevel feature, fg(Iˆ; Θg), for the query image against a reference aerial image feature, fa(l; Θa), at location l, using Euclidean distance ‖fa(l; Θa) − fg(Iˆ; Θg)‖2.” ([Workman 等, 2015, p. 4](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=4&annotation=8W4AY4ZK)) 定位过程的数学表示，提取特征后怎样找到对应的航空影像  
计算欧式距离

“We represent the localization results using a cumulative graph of the percentage of correctly localized images as a function of the percentage of candidates searched.” ([Workman 等, 2015, p. 4](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=4&annotation=CPE3DIEQ)) Reacall@K指标的具体解释

“The AlexNet architecture [20] consists of five convolutional layers (interspersed with dropout, pooling, and local response normalization layers) and three fully-connected layers (called ‘fc6’, ‘fc7’, and, the output layer, ‘fc8’). The only difference with Places is the dimensionality of the output layer (205 versus 1000 possible categorical labels).” ([Workman 等, 2015, p. 5](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=5&annotation=XPRAILHN)) 模型的基础架构由AlexNet改成，只有输出层有部分区别

“We refer to this model as CVPlaces.” ([Workman 等, 2015, p. 5](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=5&annotation=YAKNZ2QD)) 经过跨视角训练处理的Places模型

“The top feature layer from each individual network is concatenated and used as input to a final fully-connected layer with a 205 dimensional output.” ([Workman 等, 2015, p. 5](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=5&annotation=D2KG2347)) 不同尺度特征提取网络的结果最终会被融合到一起

“with the weights for our best single-scale network and randomly initialize the output layer” ([Workman 等, 2015, p. 5](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=5&annotation=25JXN2LW)) 每个网络的初始化过程

“Figure 7 shows a set of images that resulted in the maximum activation for particular ‘fc8’ nodes of each network.” ([Workman 等, 2015, p. 6](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=6&annotation=J2UR56IM)) 通过观察节点的激活值，来分析这个节点识别到了什么场景类别中的特定图像

“we learn to predict features extracted from ground-level imagery from aerial imagery of the same location.” ([Workman 等, 2015, p. 7](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=7&annotation=L49NUQIH)) 方法核心原理

“Our focus was learning the optimal parameters, Θa, for extracting features from aerial imagery.” ([Workman 等, 2015, p. 7](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=7&annotation=KNZ26RAV))

“finding better initial values for Θa is an interesting area for future work.” ([Workman 等, 2015, p. 8](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=8&annotation=RPIGZ5S6)) 此论文提出时未来工作发展

“the ground-level query image was captured in a location that is distinctive from above” ([Workman 等, 2015, p. 8](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=8&annotation=UCC7XTBM)) 精确定位，地面图像满足的条件

“Therefore, it is useful to consider the proposed approach as a pre-processing step to a more expensive matching process.” ([Workman 等, 2015, p. 8](zotero://select/library/items/XY3HAMKB)) ([pdf](zotero://open-pdf/library/items/2GEL8PA6?page=8&annotation=DE7HKCGJ)) 本论文提出的跨视角训练方法作为预处理更能有效帮助实现地理定位