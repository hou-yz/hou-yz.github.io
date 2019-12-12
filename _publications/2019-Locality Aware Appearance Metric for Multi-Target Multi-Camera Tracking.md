---
title: "Locality Aware Appearance Metric for Multi-Target Multi-Camera Tracking"
collection: publications
permalink: /publication/2019-Locality Aware Appearance Metric for Multi-Target Multi-Camera Tracking
excerpt: 'We find a inherent gap between multi-target multi-camera tracking (MTMCT) and re-identification (re-ID). Re-ID matches globally, whereas MTMCT only needs to match with a local region. To fit the local matching procedure in MTMCT, in this work, we introduce locality aware appearance metric (LAAM), that can be deployed on top of several globally learned appearance features.'
date: 2019-11-27
venue: 'arXiv'
paperurl: 'https://arxiv.org/abs/1911.12037'
citation: '@article{hou2019locality,
  title={Locality Aware Appearance Metric for Multi-Target Multi-Camera Tracking},
  author={Hou, Yunzhong and Zheng, Liang and Wang, Zhongdao and Wang, Shengjin},
  journal={arXiv preprint arXiv:1911.12037},
  year={2019}
}'
---
Multi-target multi-camera tracking (MTMCT) systems track targets across cameras. Due to the continuity of target trajectories, tracking systems usually restrict their data association within a local neighborhood. In single camera tracking, local neighborhood refers to consecutive frames; in multi-camera tracking, it refers to neighboring cameras that the target may appear successively. For similarity estimation, tracking systems often adopt appearance features learned from the re-identification (re-ID) perspective. Different from tracking, re-ID usually does not have access to the trajectory cues that can limit the search space to a local neighborhood. Due to its global matching property, the re-ID perspective requires to learn global appearance features. We argue that the mismatch between the local matching procedure in tracking and the global nature of re-ID appearance features may compromise MTMCT performance.

To fit the local matching procedure in MTMCT, in this work, we introduce locality aware appearance metric (LAAM). Specifically, we design an intra-camera metric for single camera tracking, and an inter-camera metric for multi-camera tracking. Both metrics are trained with data pairs sampled from their corresponding local neighborhoods, as opposed to global sampling in the re-ID perspective. We show that the locally learned metrics can be successfully applied on top of several globally learned re-ID features. With the proposed method, we report new state-of-the-art performance on the DukeMTMC dataset, and a substantial improvement on the CityFlow dataset.

