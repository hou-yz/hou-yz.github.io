---
title: "Learning to Structure an Image with Few Colors"
collection: publications
permalink: /publication/2019-cvpr2020-colorcnn
author: '**Yunzhong Hou**, Liang Zheng, Stephen Gould'
excerpt: 'We investigate compression for machine perception, the philosophy of which iscomparable to compression for human perception. Specifically, we restrict the color space to an extremely small size (only 1-bit image color), and then propose a CNN network to preserve the informative sturctures in an image. As opposed to the traditional clustering formulation, the proposed architecture, ColorCNN, formulates the color quantization problem as per-pixel classification. ColorCNN can be trained together with a classifier in an end-to-end manner. The quantization result from ColorCNN can achieve 82.1% accuracy with only 1-bit color on CIFAR-10, outperform the traditional quantization methods by a large margin. '
date: 2020-02-27
venue: 'CVPR'
# paperurl: 'https://arxiv.org/abs/1911.12037'
# citation: '@article{hou2019locality,
#   title={Locality Aware Appearance Metric for Multi-Target Multi-Camera Tracking},
#   author={Hou, Yunzhong and Zheng, Liang and Wang, Zhongdao and Wang, Shengjin},
#   journal={arXiv preprint arXiv:1911.12037},
#   year={2019}
# }'
---
**Yunzhong Hou**, Liang Zheng, Stephen Gould

Color and structure are the two pillars that construct an image. Usually, the structure is well expressed through a rich spectrum of colors, allowing objects in an image to be recognized by neural networks. However, under extreme limitations of color space, the structure tends to vanish, and thus a neural network might fail to understand the image. Interested in exploring this interplay between color and structure, we study the scientific problem of identifying and preserving the most informative image structures while constraining the color space to just a few bits, such that the resulting image can be recognized with possibly high accuracy. To this end, we propose a color quantization network, ColorCNN, which learns to structure the images from the classification loss in an end-to-end manner. Given a color space size, ColorCNN quantizes colors in the original image by generating a color index map and an RGB color palette. Then, this color-quantized image is fed to a pre-trained task network to evaluate its performance. In our experiment, with only a 1-bit color space (i.e., two colors), the proposed network achieves 82.1% top-1 accuracy on the CIFAR10 dataset, outperforming traditional color quantization methods by a large margin. For applications, when encoded with PNG, the proposed color quantization shows superiority over other image compression methods in the extremely low bit-rate regime. 

![alt text](/images/ColorCNN_system.png "System overview of image color quantization with ColorCNN.")

---
[paper](http://openaccess.thecvf.com/content_CVPR_2020/papers/Hou_Learning_to_Structure_an_Image_With_Few_Colors_CVPR_2020_paper.pdf)

[code](https://github.com/hou-yz/color_distillation)

---
citation:
```
@inproceedings{hou2020learning,
  title={Learning to Structure an Image with Few Colors},
  author={Hou, Yunzhong and Zheng, Liang and Gould, Stephen},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={10116--10125},
  year={2020}
}
```