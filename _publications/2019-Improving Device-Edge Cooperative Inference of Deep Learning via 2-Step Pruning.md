---
title: "Improving Device-Edge Cooperative Inference of Deep Learning via 2-Step Pruning"
collection: publications
permalink: /publication/2019-Improving Device-Edge Cooperative Inference of Deep Learning via 2-Step Pruning
author: 'Wenqi Shi, **Yunzhong Hou**, Sheng Zhou, Zhisheng Niu, Yang Zhang, and Lu Geng'
excerpt: 'This paper proposes a novel 2-step pruning method that can drastically decrease the bandwitdh requirement for transimitting feature map from given layer. In such cases, the network can be partially deployed on mobile devices without increasing bandwidth requirement.'
date: 2019-03-08
venue: 'Infocom workshop on IECOO'
# paperurl: 'https://arxiv.org/abs/1903.03472'
# citation: '@article{shi2019improving,
#   title={Improving Device-Edge Cooperative Inference of Deep Learning via 2-Step Pruning},
#   author={Shi, Wenqi and Hou, Yunzhong and Zhou, Sheng and Niu, Zhisheng and Zhang, Yang and Geng, Lu},
#   journal={arXiv preprint arXiv:1903.03472},
#   year={2019}
# }'
---
Wenqi Shi, **Yunzhong Hou**, Sheng Zhou, Zhisheng Niu, Yang Zhang, and Lu Geng

Deep neural networks (DNNs) are state-of-the-art solutions for many machine learning applications, and have been widely used on mobile devices. Running DNNs on resource-constrained mobile devices often requires the help from edge servers via computation offloading. However, offloading through a bandwidth-limited wireless link is non-trivial due to the tight interplay between the computation resources on mobile devices and wireless resources. Existing studies have focused on cooperative inference where DNN models are partitioned at different neural network layers, and the two parts are executed at the mobile device and the edge server, respectively. Since the output data size of a DNN layer can be larger than that of the raw data, offloading intermediate data between layers can suffer from high transmission latency under limited wireless bandwidth. In this paper, we propose an efficient and flexible 2-step pruning framework for DNN partition between mobile devices and edge servers. In our framework, the DNN model only needs to be pruned once in the training phase where unimportant convolutional filters are removed iteratively. By limiting the pruning region, our framework can greatly reduce either the wireless transmission workload of the device or the total computation workload. A series of pruned models are generated in the training phase, from which the framework can automatically select to satisfy varying latency and accuracy requirements. Furthermore, coding for the intermediate data is added to provide extra transmission workload reduction. Our experiments show that the proposed framework can achieve up to 25.6$\times$ reduction on transmission workload, 6.01$\times$ acceleration on total computation and 4.81$\times$ reduction on end-to-end latency as compared to partitioning the original DNN model without pruning.

![alt text](/images/2-step_pruning.png "Device-edge cooperative inference")

---
[paper](https://arxiv.org/pdf/1903.03472.pdf)

[code](https://github.com/hou-yz/pytorch-pruning-2step)

---
citation:
```
@article{shi2019improving,
  title={Improving Device-Edge Cooperative Inference of Deep Learning via 2-Step Pruning},
  author={Shi, Wenqi and Hou, Yunzhong and Zhou, Sheng and Niu, Zhisheng and Zhang, Yang and Geng, Lu},
  journal={arXiv preprint arXiv:1903.03472},
  year={2019}
}
```