# CityWall3D: A Large-Scale UAV Point Cloud Dataset for Semantic Segmentation of *Ming City Wall*

This is the official repository of the **CityWall3D** dataset. For details, please refer to:<br />
**CityWall3D: A Large-Scale UAV Point Cloud Dataset for Semantic Segmentation of *Ming City Wall*** <br />
Lin Zhao, Chaodong Ma, Xin Xu, Zequn Zhang, Nanxi Jin, Zihao Huang, Shan Liu, Qinyu Zhang, Tengping Jiang, Yongjun Wang<br />

## Abstract
Fine-grained scene understanding in the context of 3D point clouds for urban heritage environment carries enormous economic values, but its development is severely limited by the lack of suitable and specific datasets. Besides, most of the work trained on existing urban point cloud datasets exhibit poor generalization on heritage data because of a large domain gap caused by non-overlapped special and rare categories, e.g., city walls and ancient buildings. To release the potential of supervised deep learning models in 3D urban heritage understanding, we present a new point cloud benchmark, dubbed CityWall3D, with large-scale richly annotated points. Specifically, CityWall3D is the first heritage-specific 3D dataset for semantic segmentation. It covers a total length of approximately 22 kilometers of Ming City Wall and its surroundings, acquired by Unmanned Aerial Vehicle (UAV) photogrammetry, with 0.6 billion points finely labeled into 11 classes. The experimental results indicate that CityWall3D effectively represents real urban heritage environments, and poses challenges in terms of cross domain, class imbalance and density inhomogeneity of point clouds.

## Demo



## Download
If you would like to apply for this dataset, please complete the information in the following format and email it to 221302150@njnu.edu.cn or 231312003@njnu.edu.cn. We'll get right back to you. <br />
  
	Subject: Request for CityWall3D dataset 
 
    ******** Basic information ********
    · Name:
    · Email Address:
    · Affiliation/Unit:
    · Contact Phone Number:
    
    ******* Research background *******
    · Research area/direction:
    · How do you plan to use the dataset? (e.g. academic research, business analysis, curriculum projects, etc.):
    · Would you be willing to cite or refer to this dataset and its sources in your research results:
    · Your suggestions for this dataset(Optional):

## Dataset

### Overview

CityWall3D contains about 22 km of Ming City Wall, as well as the surroundings within a range of 50 meters on both sides, with a total area about 3.6 km², and the number of labeled point clouds is around 0.6 billion. 

<p align="center"> <img src="imgs/1.jpg" width="100%"> </p>
<p align="center">Figure 1. Overview of the coverage area of CityWall3D.</p> 

### Data Collection

To effectively represent the real urban heritage environment, we captured the nearly intact ontology of Ming City Wall heritage environment. Due to the complicated appearance of the city wall and the existence of scanning blind zones, CityWall3D was acquired by UAV photogrammetry. Specifically, we adopted the DJI Phantom 4 RTK UAV carrying a camera with 20 million effective pixels. During the flight, the UAV was kept at a height of about 100m over the city wall and flew along a curved trajectory. At the same time, the camera maintained a vertical shooting mode and took color images according to a certain overlap (about 70% in the heading direction and 60% in the side direction). Next, we estimated the pose and position of the camera at each viewpoint by analyzing the feature point matches between images, and generated a point cloud model by converting the feature points to 3D points.

### Semantic Annotations

<p align="center"> <img src="imgs/2.jpg" width="100%"> </p>
<p align="center">Figure 2. Examples of CityWall3D, and different semantic classes are labeled by different colors.</p> 

- **Ground** (impervious surfaces and rough terrain)
- **lnterchange** (elevated interchange and cloverleaf interchange)
- **City Wall** (heritage city walls)
- **Modern Building** (residential, high-rises, and warehouses)
- **Ancient Building** (ancient style heritage buildings)
- **Vegetation** (trees, shrubs, hedges, and bushes)
- **Car** (cars, trucks, and buses)
- **Pole** (power line poles and light poles)
- **Lantern** (ancient style lights on the city wall)
- **Water** (rivers and water canals)
- **Other** (remaining objects)

### Statistics
<p align="center"> <img src="imgs/3.jpg" width="50%"> </p>
<p align="center">Figure 3. The distribution of different semantic labels in the CityWall3D dataset.</p> 

## Updates


## Related Repos
1. [KPConv: Flexible and deformable convolution for point clouds](https://github.com/HuguesTHOMAS/KPConv) ![GitHub stars](https://img.shields.io/github/stars/HuguesTHOMAS/KPConv.svg?style=flat&label=Star)
2. [RandLA-Net: Efficient Semantic Segmentation of Large-Scale Point Clouds](https://github.com/QingyongHu/RandLA-Net) ![GitHub stars](https://img.shields.io/github/stars/QingyongHu/RandLA-Net.svg?style=flat&label=Star)
3. [SCF-Net: Learning Spatial Contextual Features for Large-Scale Point Cloud Segmentation](https://github.com/leofansq/SCF-Net) ![Github stars](https://img.shields.io/github/stars/leofansq/SCF-Net.svg?style=flat&label=Star)
4. [Push-the-Boundary: Boundary-aware Feature Propogation for Semantic Segmentation of 3D Point Clouds](https://github.com/shenglandu/PushBoundary) ![Github stars](https://img.shields.io/github/stars/shenglandu/PushBoundary.svg?style=flat&label=Star)
5. [SQN: Weakly-Supervised Semantic Segmentation of Large-Scale 3D Point Clouds](https://github.com/QingyongHu/SQN) ![GitHub stars](https://img.shields.io/github/stars/QingyongHu/SQN.svg?style=flat&label=Star)
6. [All Points Matter: Entropy-Regularized Distribution Alignment for Weakly-supervised 3D Segmentation](https://github.com/LiyaoTang/ERDA) ![Github stars](https://img.shields.io/github/stars/LiyaoTang/ERDA.svg?style=flat&label=Star)
7. [PointCT: Point Central Transformer Network for Weakly-supervised Point Cloud Semantic Segmentation](https://github.com/anhthuan1999/PointCT) ![Github stars](https://img.shields.io/github/stars/anhthuan1999/PointCT.svg?style=flat&label=Star)
