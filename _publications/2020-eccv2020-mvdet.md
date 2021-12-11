---
title: "Multiview Detection with Feature Perspective Transformation"
collection: publications
permalink: /publication/2020-eccv2020-mvdet
author: '**Yunzhong Hou**, Liang Zheng, Stephen Gould'
# excerpt: 'We incorporate multiple camera views for pedestrian detection in heavy occluded scenes. Specifically, we propose an anchor-free fully convolutional multiview detector, MVDet, that relies on feature map perspective transformation. In addition, we create a novel synthetic dataset, MultiviewX, for additional evaluation.'
date: 2020-07-14
venue: 'ECCV'
---


**Yunzhong Hou**, Liang Zheng, Stephen Gould


Incorporating multiple camera views for detection alleviates the impact of occlusions in crowded scenes. In a multiview system, we need to answer two important questions when dealing with ambiguities that arise from occlusions. First, how should we aggregate cues from the multiple views? Second, how should we aggregate unreliable 2D and 3D spatial information that has been tainted by occlusions? To address these questions, we propose a novel multiview detection system, MVDet. For multiview aggregation, existing methods combine anchor box features from the image plane, which potentially limits performance due to inaccurate anchor box shapes and sizes. In contrast, we take an anchor-free approach to aggregate multiview information by projecting feature maps onto the ground plane (bird's eye view). To resolve any remaining spatial ambiguity, we apply large kernel convolutions on the ground plane feature map and infer locations from detection peaks. Our entire model is end-to-end learnable and achieves 88.2% MODA on the standard Wildtrack dataset, outperforming the state-of-the-art by 14.1%. We also provide detailed analysis of MVDet on a newly introduced synthetic dataset, MultiviewX, which allows us to control the level of occlusion. 

Wildtrack             |  MultiviewX
:-------------------------:|:-------------------------:
![alt text](/images/eccv2020_mvdet_wildtrack_demo.gif "Detection results on Wildtrack dataset")  |  ![alt text](/images/eccv2020_mvdet_multiviewx_demo.gif "Detection results on MultiviewX dataset")

![alt text](/images/eccv2020_mvdet_architecture.png "Architecture for MVDet")

---
[paper](https://arxiv.org/abs/2007.07247)

[code](https://github.com/hou-yz/MVDet)

[知乎](https://zhuanlan.zhihu.com/p/196771711)

[MultiviewX dataset download](https://1drv.ms/u/s!AtzsQybTubHfgP9BJt2g7R_Ku4X3Pg?e=GFGeVn)

---
citation:
```
@inproceedings{hou2020multiview,
  title={Multiview Detection with Feature Perspective Transformation},
  author={Hou, Yunzhong and Zheng, Liang and Gould, Stephen},
  booktitle={ECCV},
  year={2020}
}
```