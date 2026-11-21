# 注释  
(2026/11/21 11:05:47)

“. The primary challenge is to learn the robust feature against large viewpoint changes.” ([Zheng 等, 2020, p. 1](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=1&annotation=44H7D4BR)) 该benchmarch提出的原因

“Existing benchmarks can help, but are limited in the number of viewpoints.” ([Zheng 等, 2020, p. 1](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=1&annotation=Y5DKRMNP)) 现有数据集的缺陷

“we argue that drones could serve as the third platform to deal with the geo-localization problem.” ([Zheng 等, 2020, p. 1](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=1&annotation=IDA3JXFM)) 本文的主要贡献

“The limited two viewpoints in the training set may also compromise the model to learn the viewpoint-invariant feature.” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=EZ8BC7EG)) 仅有两个视角会带来的弊端

“because drones could be motivated to capture rich information of the target place” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=8LWNCCL4)) 选用无人机视角的优点

“with few obstacles” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=5RDXXT4M))

“which results in 54 droneview images for every place in our dataset” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=527YBZHM)) 数据集构成

“Third, it is large-scale, containing 50, 218 training images in total, and has 71.64 images per class on average.” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=3YRT6ECF)) 数据集详细组成

“The images in the benchmark are captured over 1, 652 buildings of 72 universities.” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=34BHTTIX))

“Drone-view target localization. (Drone → Satellite)” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=PELM2N49))

“Drone navigation. (Satellite → Drone)” ([Zheng 等, 2020, p. 2](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=2&annotation=HZ5EIVNK))

“including scale and viewpoint variants” ([Zheng 等, 2020, p. 3](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=3&annotation=Z82IG22I)) 无人捕获到的图片信息的特点

“One line of works focuses on metric learning and builds the shared space for the images collected from different platforms.” ([Zheng 等, 2020, p. 3](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=3&annotation=S5LN3KM3))

“we select the buildings on the campus as the target, which is closer to the real-world practice.” ([Zheng 等, 2020, p. 3](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=3&annotation=4UREARK9)) 选择校园建筑的原因

“the 3D models provided by Google Earth to simulate the real drone camera” ([Zheng 等, 2020, p. 3](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=3&annotation=4LKCQ5Q9)) 并非真正使用无人机，只是模拟

“image search engine” ([Zheng 等, 2020, p. 3](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=3&annotation=R2JVPJE8)) 使用搜索引擎来拓展地面图像库

“images collected from Google Image only serve as an extra training set but a test set” ([Zheng 等, 2020, p. 4](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=4&annotation=LXTE7RK3)) 谷歌图片只用于训练

“1 satellite-view image, 1 drone-view video, and 3.38 real street-view images on average” ([Zheng 等, 2020, p. 4](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=4&annotation=GGA5GQGU))

“, and 250 buildings that lack either 3D model or street-view images.” ([Zheng 等, 2020, p. 4](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=4&annotation=8ESJNGYF)) 并非所有建筑都有完整的三列视角图像

“The rest 250 buildings are added to the gallery as distractors” ([Zheng 等, 2020, p. 4](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=4&annotation=5WJPA8ZM)) 这 250 栋建筑是**“只进候选库、不进查询集、也不进训练集”的负样本**。作用是把检索评测从“干净的小范围匹配”变成“接近真实场景的大海捞针”，同时防止模型走捷径。仅用于测试阶段

“we could view every place as one class to train a classification model” ([Zheng 等, 2020, p. 5](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=5&annotation=2DURIDSF)) **把 701 个地点当成 701 个类别**。训练时每张图都知道自己属于哪一栋楼，于是可以直接用最普通的分类器:给一张图，预测它属于 701 类中的哪一类。分类正确，就说明这个地点的特征被学出来了。

“Wshar e provides a soft constraint on the high-level features” ([Zheng 等, 2020, p. 5](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=5&annotation=933XUGQR)) Fs​、Fd​、Fg​ 三个网络看到的底层图案完全不同（正俯视的屋顶网格 / 斜俯视 / 平视街景），它们各自吐出的 512 维向量原本**不在同一个坐标系里、不可直接比较**；而 Wshare​ 定义了统一坐标系，凡是能被它正确分类的特征，就都用这套坐标表示，于是变得可比了

“we train the baseline model and extract the visual features of three kinds of data.” ([Zheng 等, 2020, p. 6](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=6&annotation=J7MMTPAA))

“Model-II has achieved better Rank@1 and AP accuracy for drone navigation (Satellite → Drone). It is not surprising since Model-II is only trained on the drone-view and satellite-view data. 2). Model-III, which fully utilizes all annotated data, has achieved the best performance in the three of all four tasks. It could serve as a strong baseline for multiple tasks.” ([Zheng 等, 2020, p. 8](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=8&annotation=6C4FRTVG))

“push the state-of-the-art performance but to show the flexibility of the proposed baseline,” ([Zheng 等, 2020, p. 8](zotero://select/library/items/KHJ8IZDL)) ([pdf](zotero://open-pdf/library/items/ZYKEJ4ML?page=8&annotation=YH3PRE2E))