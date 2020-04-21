# Maize Tassels Counting Dataset
![maize tassels](maize_tassels.png)

This repository describes the Maize Tassels Counting (MTC) dataset presented in our work:

**[TasselNet: counting maize tassels in the wild via local counts regression network](https://plantmethods.biomedcentral.com/track/pdf/10.1186/s13007-017-0224-0)**

[Hao Lu](https://sites.google.com/site/poppinace/)<sup>1</sup>, Zhiguo Cao<sup>1</sup>, Yang Xiao<sup>1</sup>, Bohan Zhuang<sup>2</sup>, [Chunhua Shen](http://cs.adelaide.edu.au/~chhshen/)<sup>2</sup>

<sup>1</sup>Huazhong University of Science and Technology, China

<sup>2</sup>The University of Adelaide, Australia

## Highlights
- 361 field images collected from 4 experimental fields across China: Zhengzhou, Henan Province, China, Taian, Shandong Province, China, Gucheng, Hebei Province, China, and Jalaid, Sinkiang Autonomous Region, China.
- Six cultivars of maize plants: Jundan No.20, Nongda, No.108, Wuyue No.3, Zhengdan No.32, Jidan No.20, and Tianlong No.9.
- Each instance is labeled with dotted annotatations.
- The dataset is full of intrinsic and extrinsic variations, shown below.

![maize tassels](challenges.jpg)

## Introduction
We first address plant-related counting problem under unconstrained field conditions. Plant counting is very challenging. What makes plants different from other conventional objects, such as crowd, cells and vehicles, is their physical size variations. This attributes to the self-changing nature of plants due to their growth over time. The size variations are also nonuniform in images. Maize tassels have almost all necessary characteristics that a typical plant has. We thus collect and annotate the MTC dataset and believe it will be a good study case for in-field plant counting problems.

## Benchmark Results
| Method        | Venue, Year           | Pretrained    | MAE   | MSE    |
| :--:          | :--:                  | :--:          | :--:  | :--:   |
| [JointSeg](https://www.sciencedirect.com/science/article/abs/pii/S1537511015304438)      | BIOSYSENG 2016        | -             | 24.2  | 31.6   | 
| [mTASSEL](https://www.sciencedirect.com/science/article/pii/S0168169915002537)       | COMPAG 2015           | -             | 19.6  | 26.1   |
| [DensityReg](http://papers.nips.cc/paper/4043-learning-to-count-objects-in-images)    | NIPS 2010 | - | 11.9 | 14.8 |
| [TasselNet](https://link.springer.com/article/10.1186/s13007-019-0537-2)         | PLME 2017            | No         | 6.6  | 9.6   |
| [CSRNet](http://openaccess.thecvf.com/content_cvpr_2018/html/Li_CSRNet_Dilated_Convolutional_CVPR_2018_paper.html) | CVPR 2018 | VGG16 | 9.4 | 14.4 |
| [S-DCNet](http://openaccess.thecvf.com/content_ICCV_2019/html/Xiong_From_Open_Set_to_Closed_Set_Counting_Objects_by_Spatial_ICCV_2019_paper.html) | ICCV 2019 | VGG16 | 5.6 | 9.1 |
| [BCNet](https://ieeexplore.ieee.org/abstract/document/8846229)         | TCSVT 2019            | VGG16         | 5.4  | 9.6   |
| [TasselNetv2](https://link.springer.com/article/10.1186/s13007-019-0537-2)         | PLME 2019            | No         | 5.4  | 8.8   |

## Downloads
[Baidu Yun (1.6GB)](https://pan.baidu.com/s/1LL9tXKHvpisDENGOsP7zWw) code: diin

[Google Drive (1.6GB)](https://drive.google.com/open?id=0B3VP9kTetyv1OXhDdTBwUER2NGM)

* Each image is associated with a standalone ".mat" annotation file that records the position of dots. The ".mat" files are created in Matlab.

* IMPORTANT NOTICE:
    - The dataset is restricted to academic purposes only.
    - If you are interested in comericial use of TasselNet, please contact Prof. Zhiguo Cao (zgcao@hust.edu.cn).

## Citation
If you find this dataset useful for your research, please cite:
```
@article{lu2017tasselnet,
  title={TasselNet: counting maize tassels in the wild via local counts regression network},
  author={Lu, Hao and Cao, Zhiguo and Xiao, Yang and Zhuang, Bohan and Shen, Chunhua},
  journal={Plant Methods},
  volume={13},
  number={1},
  pages={79},
  year={2017},
  publisher={BioMed Central}
}
```
