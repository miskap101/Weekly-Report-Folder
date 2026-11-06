# 注释  
(2026/11/6 19:07:55)

“this results in distorted images which then have to be rectified” ([Deuser 等, 2023, p. 1](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=1&annotation=ZIKBX3TF)) 极坐标变换的负面影像

“Adding hard negatives to the training batch” ([Deuser 等, 2023, p. 1](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=1&annotation=YPSK34W6))

“the default loss functions in geo-localisation it is difficult to include them.” ([Deuser 等, 2023, p. 1](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=1&annotation=S2G5EJYH)) motivation

“based on contrastive learning with symmetric InfoNCE loss” ([Deuser 等, 2023, p. 1](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=1&annotation=7JV9EAZI)) 架构的基础

“The first explicitly exploits geographically neighboring locations to provide a good starting point. The second leverages the visual similarity between the image embeddings in order to mine hard negative samples.” ([Deuser 等, 2023, p. 1](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=1&annotation=I4Y9W65E)) 两种采样策略的具体作用

“urban canyon effect” ([Deuser 等, 2023, p. 1](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=1&annotation=XXA67X8I))

“with visual clues such as sun position and the resulting shadows [3, 4, 5] or weather” ([Deuser 等, 2023, p. 1](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=1&annotation=XCCQ64Z8))

“is prone to model collapsing when hard negatives are used” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=SXLJ5RE6)) 使用负样本可能带来的弊端

“we present a weight-sharing Siamese CNN that learns class-agnostic embeddings based on the InfoNCE loss” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=QH4PVUAU)) 一对结构相同的网络，分别吃两张图、各吐一个特征向量，再比相似度  
不依赖任何地点类别标签，模型学习的是度量空间  
InfoNCE 这个对比损失训练出来的：它让正样本对（同地点）相似度最大、与 batch 内所有负样本相似度最小

“are hard to distinguish for the model from positives examples” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=RGXEK9HA)) 两种sampling提出的motivation

“a key ingredient” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=SWZUACI4))

“contrast close geographic neighbours as a good initialisation” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=H4MZ6L7I))

“focus on hard negatives examples” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=YEWULYJD))

“applied polar transformation to the satellite image” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=UG9K4XMJ)) 极坐标变换作为常见的预处理技术

“the disadvantage that the distortion injects disturbances into the image” ([Deuser 等, 2023, p. 2](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=2&annotation=37RHJNNM))

“Triplet loss aims to decrease the distance between a positive example and an anchor, while increasing the distance between a negative example and the anchor” ([Deuser 等, 2023, p. 3](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=3&annotation=HFEZNWWG)) 三元组损失的具体作用

“showed the advantage of using two negatives as quadruple loss instead of a triplet” ([Deuser 等, 2023, p. 3](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=3&annotation=JCE2N4K8))

“A symmetric formulation showed to be useful in multi-modal pre-training [30] to bridge the gap between the modalities” ([Deuser 等, 2023, p. 3](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=3&annotation=ZBZ9XC9L)) 采用对称公式的原因

“a positive example is always contrasted with N-1 negative examples” ([Deuser 等, 2023, p. 3](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=3&annotation=Z3AW7EB9))

“a custom sampler” ([Deuser 等, 2023, p. 3](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=3&annotation=QN9FDMJM)) 针对多个正样本的处理方法

“Vision-Transformer [24, 22, 23] or MLP mixer architectures” ([Deuser 等, 2023, p. 3](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=3&annotation=MA8METJB)) 还需要与transformer和MLP架构进行对比

“While current work does not use weight-sharing due to the different view-domains, we emphasise the use of a weight-shared ConvNeXt as a single encoder for both views.” ([Deuser 等, 2023, p. 4](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=4&annotation=LQTCL2SD)) **不是"两个结构相同的网络"，而是"同一个网络跑了两遍"**，参数共享的真实含义​

“near neighbours” ([Deuser 等, 2023, p. 4](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=4&annotation=7AI65V78)) **把地理相近的位置，当作天然的难负样本**

“based on the haversine distance” ([Deuser 等, 2023, p. 4](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=4&annotation=69FVLFNU)) 选择依据

“These K neighbours are sorted based on their similarity and then k 2 nearest samples are selected for the batch, the remaining k 2 samples are randomly selected from the remaining samples in K.” ([Deuser 等, 2023, p. 4](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=4&annotation=XPLKXKN6)) 最近邻选择策略

“1 : n mapping” ([Deuser 等, 2023, p. 5](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=5&annotation=84S32L3G)) 与前面两个数据集不同的地方

“same-area and cross-area” ([Deuser 等, 2023, p. 5](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=5&annotation=RLK6S3C8))

“all approaches naturally have problems to distinguish between the semi-positives and the ground truth image as they are very close to each other.” ([Deuser 等, 2023, p. 5](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=5&annotation=SNPZ53EF)) 普遍存在的问题，难以区分半正例和真实图像

“Vision Transformers are not capable of dealing with multiple input sizes due to their fixed size positional encoding.” ([Deuser 等, 2023, p. 7](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=7&annotation=FP24S2AT)) vit处理图像大小的限制

“additional datasets with explicitly not aligned central positions and unknown geographical orientation between satellite and street-view image are required” ([Deuser 等, 2023, p. 8](zotero://select/library/items/H4UJT7XW)) ([pdf](zotero://open-pdf/library/items/M5QWJS8Z?page=8&annotation=N2TII739)) 经典数据集测试已经饱和，需要更多样性的数据集提出