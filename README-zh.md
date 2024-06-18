# CityWall3D：用于明城墙语义分割的大规模无人机点云数据集

这是**CityWall3D**数据集的官方库。详情请参考:<br />
**CityWall3D: A Large-Scale UAV Point Cloud Dataset for Se-mantic Segmentation of *Ming City Wall*** <br />
Lin Zhao, Chaodong Ma, Xin Xu, Zequn Zhang, Nanxi Jin, Zihao Huang, Shan Liu, Qinyu Zhang, Tengping Jiang, Yongjun Wang<br />


城市遗产环境三维点云的精细场景理解具有巨大的经济价值，但由于缺乏合适的特定数据集，其发展受到严重限制。此外，大多数在现有城市点云数据集上训练的工作在遗产数据上的泛化效果不佳，原因是城墙和古建筑等非重叠的特殊和稀有类别造成了巨大的领域差距。为了释放有监督深度学习模型在三维城市遗产理解中的潜力，我们提出了一个新的点云基准，称为 CityWall3D，其中包含大规模的丰富注释点。具体来说，CityWall3D 是首个用于语义分割的特定遗产三维数据集。该数据集涵盖总长约 22 公里的明城墙及其周边地区，由无人机（UAV）摄影测量获得，其中有 6 亿个点被精细标注为 11 个类别。实验结果表明，CityWall3D 有效地再现了真实的城市遗产环境，并在点云的跨域、类不平衡和密度不均匀性方面提出了挑战。

## 样例


## 下载
如果您想申请该数据集，请按以下格式填写信息，并通过电子邮件发送至 221302150@njnu.edu.cn 或 231312003@njnu.edu.cn。我们会尽快给您回复。 <br />
  
	主题：请求提供 CityWall3D 数据集  
 
    ******** 基本信息 ********
    · 姓名:
    · 电子邮件:
    · 所属单位:
    · 联系电话:
    
    ******** 研究背景 ********
    · 研究领域/方向:
    · 您计划如何使用数据集？（例如学术研究、商务分析、课程项目等）：:
    · 您是否愿意在您的研究成果中引用或参考该数据集及其来源:
    · 您对该数据集的建议（可选）:
    
## 数据集

### 总览

CityWall3D 包含约 22 公里的明城墙以及两侧 50 米范围内的周边环境，总面积约为 3.6 平方公里，标注点云数量约为 6 亿个。

<p align="center"> <img src="imgs/1.jpg" width="100%"> </p>
<p align="center">图 1. CityWall3D 覆盖区域概览。</p> 

### 数据收集

为了有效表现真实的城市遗产环境，我们捕捉了几乎完整的明城墙遗产环境本体。由于城墙外形复杂且存在扫描盲区，CityWall3D 采用了无人机摄影测量的方式获取。具体来说，我们采用大疆 Phantom 4 RTK 无人机，搭载 2000 万有效像素的相机。在飞行过程中，无人机保持在城墙上空约 100 米的高度沿曲线轨迹飞行。同时，摄像机保持垂直拍摄模式，并按照一定的重叠率（航向约 70%，侧向约 60%）拍摄彩色图像。接下来，我们通过分析图像之间的特征点匹配情况来估计摄像机在每个视点的姿势和位置，并通过将特征点转换为三维点来生成点云模型。

### 语义标注

<p align="center"> <img src="imgs/2.jpg" width="100%"> </p>
<p align="center">图 2. CityWall3D 示例，不同的语义类别用不同的颜色标注。</p> 

- **地面**（不透水表面和崎岖地形）
- **立交桥**（高架立交和三叶立交）
- **城墙**（遗产城墙）
- **现代建筑**（住宅、高层建筑和仓库）
- **古建筑**（古代遗产建筑）
- **植被**（树木、灌木、树篱和灌木）
- **车**（轿车、卡车和公共汽车）
- **杆**（电线杆和灯杆）
- **灯笼**（城墙上的古风路灯）
- **水系**（河流和水渠）
- **其他**（剩余对象）

### 数据统计
<p align="center"> <img src="imgs/3.jpg" width="50%"> </p>
<p align="center">图 3. CityWall3D 中不同语义类别的分布情况。</p> 


## 更新日历



## 相关库
1. [KPConv: Flexible and deformable convolution for point clouds](https://github.com/HuguesTHOMAS/KPConv) ![GitHub stars](https://img.shields.io/github/stars/HuguesTHOMAS/KPConv.svg?style=flat&label=Star)
2. [RandLA-Net: Efficient Semantic Segmentation of Large-Scale Point Clouds](https://github.com/QingyongHu/RandLA-Net) ![GitHub stars](https://img.shields.io/github/stars/QingyongHu/RandLA-Net.svg?style=flat&label=Star)
3. [SCF-Net: Learning Spatial Contextual Features for Large-Scale Point Cloud Segmentation](https://github.com/leofansq/SCF-Net) ![Github stars](https://img.shields.io/github/stars/leofansq/SCF-Net.svg?style=flat&label=Star)
4. [Push-the-Boundary: Boundary-aware Feature Propogation for Semantic Segmentation of 3D Point Clouds](https://github.com/shenglandu/PushBoundary) ![Github stars](https://img.shields.io/github/stars/shenglandu/PushBoundary.svg?style=flat&label=Star)
5. [SQN: Weakly-Supervised Semantic Segmentation of Large-Scale 3D Point Clouds](https://github.com/QingyongHu/SQN) ![GitHub stars](https://img.shields.io/github/stars/QingyongHu/SQN.svg?style=flat&label=Star)
6. [All Points Matter: Entropy-Regularized Distribution Alignment for Weakly-supervised 3D Segmentation](https://github.com/LiyaoTang/ERDA) ![Github stars](https://img.shields.io/github/stars/LiyaoTang/ERDA.svg?style=flat&label=Star)
7. [PointCT: Point Central Transformer Network for Weakly-supervised Point Cloud Semantic Segmentation](https://github.com/anhthuan1999/PointCT) ![Github stars](https://img.shields.io/github/stars/anhthuan1999/PointCT.svg?style=flat&label=Star)
