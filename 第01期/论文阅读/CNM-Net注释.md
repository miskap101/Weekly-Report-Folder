# 注释  
(2026/10/23 15:57:44)

“due to the drastic change in viewpoint” ([Hu 等, 2018, p. 7258](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=1&annotation=5QFW8K8R)) 定位问题的挑战

“based on the Siamese architecture” ([Hu 等, 2018, p. 7258](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=1&annotation=6YWZKVN7))

“first use the fully convolutional layers to extract local image features, which are then encoded into global image descriptors using the powerful NetVLAD” ([Hu 等, 2018, p. 7258](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=1&annotation=7WP6Y7NF)) 主要贡献

“a simple yet effective weighted soft margin ranking loss function” ([Hu 等, 2018, p. 7258](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=1&annotation=SAS2NDQE)) 新的损失函数

“usually do not have a comprehensive coverage of the area.” ([Hu 等, 2018, p. 7258](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=1&annotation=6JRK4VLG)) 只使用地面视角的图片无法对区域完全覆盖，具有局限性

“the drastic change in viewpoint between ground and aerial images.” ([Hu 等, 2018, p. 7258](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=1&annotation=T8HXS2ZG))

“use of the global VLAD descriptor” ([Hu 等, 2018, p. 7259](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=2&annotation=RQCPWG4F)) 使用到的方法

“The key idea is that NetVLAD aggregates the local features obtained from the CNN to form global representations that are independent of the locations of the local features.” ([Hu 等, 2018, p. 7259](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=2&annotation=TA892YNH))

“combine NetVLAD layers with a Siamese network” ([Hu 等, 2018, p. 7259](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=2&annotation=8YRVA2NU))

“learns local features and forms global descriptors” ([Hu 等, 2018, p. 7259](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=2&annotation=JHGSPTEK))

“a new weighted soft margin ranking loss” ([Hu 等, 2018, p. 7259](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=2&annotation=LSZWUA6H))

“two parts: local feature extraction and global descriptor generation.” ([Hu 等, 2018, p. 7260](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=3&annotation=TCCGJWUP))

“For a satellite image Is, the set of local features is given by Us = f L(Is; ΘsL), where ΘsL is the parameters of the FCN of the satellite branch.” ([Hu 等, 2018, p. 7260](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=3&annotation=FK7Q7KVN)) 提取卫星图像特征网络分支的相关参数

“For a ground image Ig, the set of local features Ug = f L(Ig; ΘgL), where ΘgL is the parameters of the FCN of the ground view branch.” ([Hu 等, 2018, p. 7260](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=3&annotation=KSCJDJDC)) 地面图像分支相关参数介绍

“similarity comparison.” ([Hu 等, 2018, p. 7260](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=3&annotation=UCVVEZDF))

“The global descriptor of an image can be formulated as vi = f G(Ui; ΘiG), where i ∈ {s, g} represents the satellite or ground branch.” ([Hu 等, 2018, p. 7260](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=3&annotation=HLY2BZ3G)) 整个模型的数学表达概览，把局部特征集合 U 塞进聚合函数 fG，吐出一个全局向量 v

“feeding them into the loss function for end-to-end training, or using them for similarity comparison.” ([Hu 等, 2018, p. 7260](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=3&annotation=PLBJ9BIX)) 轻量化的方法

“the two NetVLAD layers with the same number of clusters that are trained together in a Siamese-like architecture” ([Hu 等, 2018, p. 7260](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=3&annotation=Z6GZ2VVJ)) 两个 NetVLAD 不是各训各的，而是在同一个排序损失下联合优化

“achieves cross-view matching” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=GTC3PAJG)) 通过局部特征的质心将地面和卫星图像匹配

“because they are only relative to the centroids” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=56N8XJ46)) 残差只相对于重心

“the descriptor vector of each centroid is the summation of residuals to the centroid” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=B3LECNJX)) 相对中心的偏差之和，不是特征本身

“The global descriptor of the satellite image is given by vs = f G(f L(Is; ΘsL); ΘsG) and ground image is given by vg = f G(f L(Ig; ΘgL); ΘgG).” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=LJ3Q8QCU)) 两个函数嵌套：fL 是 VGG16 卷积部分（图像 → 局部特征 U），fG 是 NetVLAD（U → 全局描述子 v）。

“The two branches have identical structures with different parameters” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=A453KIW4)) 不同的分支相同的结构嵌套两种函数分别对地面和卫星图像进行处理

“because weight sharing has been proven to improve metric learning in many of the Siamese network architectures” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=DQ8J9I4E)) 使用权重共享的原因

“triplet loss” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=WIPEQW59))

“for image matching and retrieval tasks” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=4JCMK47Z))

“resulted in slow convergence” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=NPAC7USE))

“force the irrelevant negative pairs further away from the positive pairs” ([Hu 等, 2018, p. 7261](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=4&annotation=PYHHK3EZ)) 四元组损失的作用

“VGG16 [38] architecture with 13 convolutional layers” ([Hu 等, 2018, p. 7262](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=5&annotation=QT3MIQCB)) 网络参数配置

“a NetVLAD with 64 clusters” ([Hu 等, 2018, p. 7262](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=5&annotation=6ARZXX98))

“two stages” ([Hu 等, 2018, p. 7262](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=5&annotation=YTKPJXXP))

“We have a total of M × 2(M − 1) triplets for M positive pairs of ground-to-satellite images.” ([Hu 等, 2018, p. 7262](zotero://select/library/items/NZKDCHA8)) ([pdf](zotero://open-pdf/library/items/DHW8SJVU?page=5&annotation=ZGXJP324)) 三元组是 (anchor, positive, negative)。一个 batch 里有 M 对配好的 (地面, 卫星)。**ground 当 anchor** 时：正样本是配对的卫星，负样本是 batch 里**其余 M−1 张卫星** → M−1 个三元组。**satellite 当 anchor** 时：反过来，负样本是其余 M−1 张地面 → 又是 M−1 个。所以每对贡献 2(M−1)，M 对共 M × 2(M−1)。**那个 2 就是"双向都当一遍 anchor"**​，这一点原文解释得绕，但本质就这么简单