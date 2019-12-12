---
title: "A Locality Aware City-Scale Multi-Camera Vehicle Tracking System"
collection: publications
permalink: /publication/2019-A Locality Aware City-Scale Multi-Camera Vehicle Tracking System
excerpt: '**Yunzhong Hou**, Heming Du, and Liang Zheng

Vehicle tracking across multiple cameras can be difficult for modern tracking systems. In order to avoid difficulties in a large scenario, we keep the tracking procedure within a minimal range. '
date: 2019-05-15
venue: 'CVPR workshop on AI-City'
# paperurl: 'http://openaccess.thecvf.com/content_CVPRW_2019/papers/AI%20City/Hou_A_Locality_Aware_City-Scale_Multi-Camera_Vehicle_Tracking_System_CVPRW_2019_paper.pdf'
# citation: '@InProceedings{Hou_2019_CVPR_Workshops,
# author = {Hou, Yunzhong and Du, Heming and Zheng, Liang},
# title = {A Locality Aware City-Scale Multi-Camera Vehicle Tracking System},
# booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
# month = {June},
# year = {2019}
# }'
---
Vehicle tracking across multiple cameras can be difficult for modern tracking systems. Given unlikely candidates and faulty similarity estimation, data association struggles at city-scale tracking. In order to avoid difficulties in a large scenario, we keep the tracking procedure within a minimal range. The benefit of this smaller scenario idea is two-fold. On the one hand, ruling out most unlikely candidates decrease the possibility of mis-assignment. On the other hand, the system can devote all its discriminative power on the remaining local candidate pool. In fact, our tracking system features two parts to keep the data association within a small range, while at the same time increase the locality awareness for smaller scenarios. First, multiple cues including spatial-temporal information and camera topology are leveraged to restrict the candidate selection. Second, the appearance similarity estimation module is carefully tuned so that it focuses on the smaller local candidate pool. Based on a minimal view for the large scenario, the proposed system finished 5-th place in the 2019 AI-City challenge for city-scale multi-camera vehicle tracking.

