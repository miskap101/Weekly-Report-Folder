# 注释  
(2026/11/6 19:08:32)

“existing learning pipelines are orientationspecific or FoV-specific, demanding separate model training for different ground view variations” ([Mi 等, 2024, p. 1](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=1&annotation=GUBZGCMG)) 现有方法存在的局限性

“Northaligned spatial correspondence and predefined FoVs in the training data” ([Mi 等, 2024, p. 1](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=1&annotation=DVXQXSKN))

“by enforcing proximity between ground view variations of the same location” ([Mi 等, 2024, p. 1](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=1&annotation=4JKUJIBB)) 提高鲁棒性和抵抗力的方法

“cyclically shifting a ground view panorama by a random angle to obtain orientation variations, or further reducing the FoV from 360◦ to 70◦, 90◦, or 180◦ to simulate limited ground view information” ([Mi 等, 2024, p. 2](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=2&annotation=A9RQII7E)) 通过位移移动地图（改变原本的北对齐）或者缩减视角提高数据集的鲁棒性

“they train and evaluate models separately for each setting” ([Mi 等, 2024, p. 2](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=2&annotation=TVIXJGKJ)) 只对特定的方向或者角度进行训练限制了泛化能力

“the models are often biased toward training data to capture specific spatial correspondence” ([Mi 等, 2024, p. 2](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=2&annotation=YL82DW78)) 模型训练的局限性从而限制了泛化，怎样设计突破这个局限性，实现更好的泛化效果？

“a robust model should capture consistent features for the same location regardless of orientations or FoVs and identify the same reference image across ground view variations” ([Mi 等, 2024, p. 2](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=2&annotation=N5DW9R3J)) 提取特征的底层原理

“its augmented counterpart” ([Mi 等, 2024, p. 3](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=3&annotation=78EC9X4W)) 增强版本是航拍分支，对同一张卫星参考图做两次独立的随机增强（论文中是随机旋转）

“mitigating potential shortcuts found in the training data” ([Mi 等, 2024, p. 3](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=3&annotation=MAHHWVEN)) 与上一段落提到的shorcut带来的负面影像对应，这里减少

“using a model-agnostic learning pipeline” ([Mi 等, 2024, p. 3](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=3&annotation=W5G7BS9D)) 通用学习方法，不拘泥于单个模型

“the trade-off between the model’s focus on geometric or semantic cues” ([Mi 等, 2024, p. 3](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=3&annotation=MFF45A38)) 对于几何和语义的选择会影响变化检测

“The standard approach uses a siamese network [2] to encode the ground view and the aerial images and optimizes a well-designed loss to align the feature embeddings.” ([Mi 等, 2024, p. 3](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=3&annotation=KQTN2KBL))

“First, specific FoV information is required for aerial image/feature cropping during both training and testing, while in real-world data this strong prior is unknown, especially during testing. Second, models trained on a specific setting cannot generalize and do not perform satisfactorily on all FoV scenarios. Thus several specialised models are trained for each setting.” ([Mi 等, 2024, p. 4](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=4&annotation=I7EFHA2I)) 对于未知方向和有限视角现有方法存在的局限性

“aims to enhance the robustness of geo-localization models by enforcing proximity between ground view variations and their original representations” ([Mi 等, 2024, p. 4](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=4&annotation=3DJUUP8S))

“can be cyclically shifted with a random angle and restricted by a specific FoV (e.g., 70◦, 90◦, 180◦, and 360◦)” ([Mi 等, 2024, p. 5](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=5&annotation=9VB4AJC3)) 地面图像的增强版本的由来

“A random orientation angle θ is first used to horizontally shift the ground image, followed by the application of a FoV angle α to crop the panorama query to a FoV query Iq∗ = Tq(Iq|θ, α).” ([Mi 等, 2024, p. 5](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=5&annotation=MLF777Z9)) 增强图像的具体操作

“produce similar representations between the original images (North-aligned, full panorama) and their transformed counterpart” ([Mi 等, 2024, p. 5](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=5&annotation=L8BVWBJ2)) 单视图对比学习的目的

“enforce the similarity between two distorted versions of the same reference image using random data augmentations, aiming to obtain more robust feature representations” ([Mi 等, 2024, p. 6](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=6&annotation=HN8Y3J43)) 航空对比损失与地面对比损失的区别，航空图像是两个是扰乱图像相似

“vanilla loss” ([Mi 等, 2024, p. 6](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=6&annotation=E2HTVKTP)) 原始损失：强调「未经修改、来自基模型」，与 ConGeo 新增的三项对比损失构成对照

“Combining all the terms previously described” ([Mi 等, 2024, p. 6](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=6&annotation=LLKVR8KG)) 集合所有损失，最终完成对比学习目标

“the orientation angle θ is randomly drawn between 0◦ and 360◦ while the FoV angle α is set to 180◦” ([Mi 等, 2024, p. 7](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=7&annotation=AH8CZP7F)) θ 管的是「朝哪个方向看」，做的是**循环平移**，不丢任何信息；α 管的是「一眼能看多宽」，做的是**裁剪**，会真的丢掉一半视野

“The total loss is a weighted summation of the four loss functions,” ([Mi 等, 2024, p. 17](zotero://select/library/items/93DEP85F)) ([pdf](zotero://open-pdf/library/items/9SDILY9W?page=17&annotation=N3R5VRHK))