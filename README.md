# Awesome_Dynamic_SLAM [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
The following paper are the papers that focuses on the **SLAM in dynamic Environments**. In the dynamic environment, there are two kinds of robust SLAM: First is **detection & removal**. Another is **detection & tracking**. Although the mapping part in dynamic environment is not my focus, but I will also put some articles yet also very interesting.

> Vision means that the pipeline is built with camera. Others are the same, such as lidar, radar, sensor fusion.

------

# Related survey papers:

- [**A survey: which features are required for dynamic visual simultaneous localization and mapping?**](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8285453/pdf/42492_2021_Article_86.pdf). Zewen Xu,CAS. 2021

- [**State of the Art in Real-time Registration of RGB-D Images**](https://cg.cs.uni-bonn.de/aigaion2root/attachments/StateoftheArtinReal-timeRegistrationofRGB-DImages.pdf). Stotko, Patrick. University of Bonn. 2016
- [**Visual SLAM and Structure from Motion in Dynamic Environments: A Survey**](https://dl.acm.org/doi/pdf/10.1145/3177853).  University of Oxford. 2018
- [**State of the Art on 3D Reconstruction with RGB-D Cameras**](https://www.cg.informatik.uni-siegen.de/data/Publications/2018/star1009-main.pdf). Michael Zollhöfer. Stanford University. 2018

# Dynamic Object Detection and *Removal*

- Pfreundschuh, Patrick, et al. “**[Dynamic Object Aware LiDAR SLAM Based on Automatic Generation of Training Data.](http://arxiv.org/abs/2104.03657)**” (*ICRA* *2021*)
  - **ETH ASL**,code, [video](https://youtu.be/LcDxd97r1Gc), [**dataset**](https://projects.asl.ethz.ch/datasets/doals), Lidar
  
- Canovas Bruce, et al. “[**Speed and Memory Efficient Dense RGB-D SLAM in Dynamic Scenes.**](https://doi.org/10.1109/IROS45743.2020.9341542)” (*IROS* 2020)
  - **GIPSA-lab**, [code](https://github.com/BruceCanovas/supersurfel_fusion), [video](https://youtu.be/hzzVVHUAO74)
  
- Yuan Xun and Chen Song. “[**SaD-SLAM: A Visual SLAM Based on Semantic and Depth Information.**](http://ras.papercept.net/images/temp/IROS/files/0092.pdf)” *(IROS 2020)*
  - **USTC**, code, video
  
- Dong, Erqun, et al. “[**Pair-Navi: Peer-to-Peer Indoor Navigation with Mobile Visual SLAM.**](https://cswu.me/papers/infocom19_pairnavi.pdf)” (ICCC 2019)
  - Tsinghua, [Code](https://github.com/Horacehxw/Dynamic_ORB_SLAM2), Video, [Slides](https://slidetodoc.com/pairnavi-peertopeer-indoor-navigation-with-mobile-visual-slam/).
  
- Ji Tete, et al. “**[Towards Real-Time Semantic RGB-D SLAM in Dynamic Environments](https://arxiv.org/abs/2104.01316v1)**.” (ICRA 2021)

- Palazzolo Emanuele, et al. “**[ReFusion: 3D Reconstruction in Dynamic Environments for RGB-D Cameras Exploiting Residuals.](https://arxiv.org/abs/1905.02082v3)**” (IROS 2019)
  - [code](https://github.com/PRBonn/refusion),[video](https://youtu.be/1P9ZfIS5-p4).University of Bonn.
  
- Arora Mehul, et al. ***[Mapping the Static Parts of Dynamic Scenes from 3D LiDAR Point Clouds Exploiting Ground Segmentation](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/arora2021ecmr.pdf)***. p. 6.

- Chen Xieyuanli, et al. “**[Moving Object Segmentation in 3D LiDAR Data: A Learning-Based Approach Exploiting Sequential Data](https://www.ipb.uni-bonn.de/pdfs/chen2021ral-iros.pdf)**.” *IEEE Robotics and Automation Letters*, 2021
  - [code](https://github.com/PRBonn/LiDAR-MOS). [video](https://www.youtube.com/watch?v=NHvsYhk4dhw). University of Bonn.
  
- Zhang Tianwei, et al. “[**FlowFusion: Dynamic Dense RGB-D SLAM Based on Optical Flow.**](http://arxiv.org/abs/2003.05102.)”(ICRA 2020)
  - code. [video](https://youtu.be/6yPGDdwKFLA).
  
- Zhang Tianwei, et al. “**[AcousticFusion: Fusing Sound Source Localization to Visual SLAM in Dynamic Environments.](http://arxiv.org/abs/2108.01246)**”,IROS 2021
  - [video](https://youtu.be/8eNikzp9LIQ). 结合声音信号
  
- 1. Liu Yubao and Miura Jun. “[**RDS-SLAM: Real-Time Dynamic SLAM Using Semantic Segmentation Methods.**](https://doi.org/10.1109/ACCESS.2021.3050617)” *IEEE Access* 2021

  2. Liu Yubao and Miura Jun. “RDMO-SLAM: Real-Time Visual SLAM for Dynamic Environments Using Semantic Label Prediction With Optical Flow.” *IEEE Access*, vol. 9, 2021, pp. 106981–97. *IEEE Xplore*, https://doi.org/10.1109/ACCESS.2021.3100426.

  - [code](https://github.com/yubaoliu/RDS-SLAM.git
    ), video.

- Cheng Jiyu, et al. “**Improving Visual Localization Accuracy in Dynamic Environments Based on Dynamic Region Removal.**” *IEEE Transactions on Automation Science and Engineering*, vol. 17, no. 3, July 2020, pp. 1585–96. *IEEE Xplore*, https://doi.org/10.1109/TASE.2020.2964938.

- Soares João Carlos Virgolino, et al. “**[Crowd-SLAM: Visual SLAM Towards Crowded Environments Using Object Detection.](https://doi.org/10.1007/s10846-021-01414-1)**” *Journal of Intelligent & Robotic Systems* 2021

  - [code](https://github.com/virgolinosoares/Crowd-SLAM), video

- Kaveti Pushyami and Singh Hanumant. “**[A Light Field Front-End for Robust SLAM in Dynamic Environments.](http://arxiv.org/abs/2012.10714)**”.

- Kuen-Han Lin and Chieh-Chih Wang. “**[Stereo-Based Simultaneous Localization, Mapping and Moving Object Tracking.](https://doi.org/10.1109/IROS.2010.5649653)**” IROS 2010

- Fu, H.; Xue, H.; Hu, X.; Liu, B. **[LiDAR Data Enrichment by Fusing Spatial and Temporal Adjacent Frames](https://doi.org/10.3390/rs13183640)**. *Remote Sens.* **2021**, *13*, 3640. 

- Qian, Chenglong, et al. ***RF-LIO: Removal-First Tightly-Coupled Lidar Inertial Odometry in High Dynamic Environments***. p. 8. IROS2021, **XJTU**

- K. Minoda, F. Schilling, V. Wüest, D. Floreano, and T. Yairi, “**[VIODE: A Simulated Dataset to Address the Challenges of Visual-Inertial Odometry in Dynamic Environments,](https://doi.org/10.1109/LRA.2021.3058073)**”RAL 2021

  - 动态环境的数据集，包括了静态，动态等级的场景，感觉适合用来作为验证。
  - 东京大学，[code](https://github.com/kminoda/VIODE)
  
- W. Dai, Y. Zhang, P. Li, Z. Fang, and S. Scherer, “**[RGB-D SLAM in Dynamic Environments Using Point Correlations](https://doi.org/10.1109/TPAMI.2020.3010942)**,” *IEEE Transactions on Pattern Analysis and Machine Intelligence*, pp. 1–1, 2020

  - 浙大，使用点的关联进行去除。

- C. Huang, H. Lin, H. Lin, H. Liu, Z. Gao, and L. Huang, “YO-VIO: Robust Multi-Sensor Semantic Fusion Localization in Dynamic Indoor Environments,” in 2021 International Conference on Indoor Positioning and Indoor Navigation (IPIN), 2021.
  - 使用yolo和光流对运动对象进行判断，去除特征点后进行定位
  - VIO的结合

- Dynamic-VINS：RGB-D Inertial Odometry for a Resource-restricted Robot in Dynamic Environments. 
  - 分割+运动点置信度，[code](https://github.com/HITSZ-NRSL/Dynamic-VINS),[video](https://www.bilibili.com/video/BV1bF411t7mx)



# Dynamic Object Detection and ***Tracking***

- “**[AirDOS: Dynamic SLAM benefits from Articulated Objects,](http://arxiv.org/abs/2109.09903)**” Qiu Yuheng, et al. 2021(Arxiv)
  - [code](https://github.com/haleqiu/airdos)(TBA), [Paper](https://arxiv.org/abs/2109.09903), Video. **CMU RI**, Vision.
  
- “[**DOT: Dynamic Object Tracking for Visual SLAM**](http://arxiv.org/abs/2010.00052).” Ballester, Irene, et al.(ICRA 2021)
  - code, [video](https://youtu.be/9hWChyQGKJk), **University of Zaragoza**, Vision
  
- Liu Yubao and Miura Jun. “[**RDMO-SLAM: Real-Time Visual SLAM for Dynamic Environments Using Semantic Label Prediction With Optical Flow**](https://doi.org/10.1109/ACCESS.2021.3100426).” *IEEE Access*. 

- Kim Aleksandr, et al. “[**EagerMOT: 3D Multi-Object Tracking via Sensor Fusion.**](http://arxiv.org/abs/2104.14682)” (*ICRA 2021*)
  - **TUM**, [code](https://github.com/aleksandrkim61/EagerMOT), [video](https://youtu.be/k8pKpvbenoM), Sensor Fusion.
  
- 1. Shan, Mo, et al. “**[OrcVIO: Object Residual Constrained Visual-Inertial Odometry.](http://moshan.cf/orcvio_githubpage/0072.pdf)**” *(IROS2020)*
  2. Shan, Mo, et al. “**[OrcVIO: Object Residual Constrained Visual-Inertial Odometry.](http://arxiv.org/abs/2007.15107)**” (IROS 2021)

  - [code](https://github.com/shanmo/OrcVIO), [video](http://moshan.cf/orcvio_githubpage/), [Project page](http://moshan.cf/orcvio_githubpage/).

- Rosen, David M., et al. “[**Towards Lifelong Feature-Based Mapping in Semi-Static Environments.**](https://doi.org/10.1109/ICRA.2016.7487237)” *(ICRA 2016)*

- 1. Henein Mina, et al. “[**Dynamic SLAM: The Need For Speed**](https://arxiv.org/abs/2002.08584v2).” *(ICRA 2020)*
  2. Zhang Jun, et al. “**[VDO-SLAM: A Visual Dynamic Object-Aware SLAM System](http://arxiv.org/abs/2005.11052)**.” (ArXiv 2020)
  3. **[Robust Ego and Object 6-DoF Motion Estimation and Tracking](https://arxiv.org/abs/2007.13993v1)**,Jun Zhang, Mina Henein, Robert Mahony and Viorela Ila. IROS 2020([code](https://github.com/halajun/multimot_track))

  - [code](https://github.com/halajun/VDO_SLAM), [video](https://drive.google.com/file/d/1PbL4KiJ3sUhxyJSQPZmRP6mgi9dIC0iu/view), Vision
  
- Minoda, Koji, et al. “**[VIODE: A Simulated Dataset to Address the Challenges of Visual-Inertial Odometry in Dynamic Environments.](https://arxiv.org/abs/2102.05965v1)**” (RAL 2021)

  - [**code_and dataset**](https://github.com/kminoda/VIODE), [video](https://youtu.be/LlFTyQf_dlo).

- Vincent, Jonathan, et al. “[**Dynamic Object Tracking and Masking for Visual SLAM.**](https://arxiv.org/abs/2008.00072v1)”, (IROS 2020)

  - [code](https://github.com/introlab/dotmask), video, 

- Huang, Jiahui, et al. “**[ClusterVO: Clustering Moving Instances and Estimating Visual Odometry for Self and Surroundings](http://arxiv.org/abs/2003.12980)**.” (CVPR 2020)

  - Tsinghua, code, [video](https://youtu.be/paK-WCQpX-Y).[slides](https://cg.cs.tsinghua.edu.cn/people/~huangjh/clustervo-slides.pdf).

- Liu, Yuzhen, et al. “**[A Switching-Coupled Backend for Simultaneous Localization and Dynamic Object Tracking.](https://github.com/zhuhu00/Awesome_Dynamic_SLAM/raw/main/pdfs/liu_2021_SwitchingCoupled.pdf)**” (RAL 2021)

  - Tsinghua

- Yang Charig, et al. “**[Self-Supervised Video Object Segmentation by Motion Grouping](http://arxiv.org/abs/2104.07658)**.”(ICCV 2021)

  - [Project page](https://charigyang.github.io/motiongroup/).

- Long Ran, et al. “**[RigidFusion: Robot Localisation and Mapping in Environments with Large Dynamic Rigid Objects](http://arxiv.org/abs/2010.10841)**.” ,(RAL 2021)

  - [**project page**](https://conferences.inf.ed.ac.uk/rigidfusion/).code, video, 

- Yang Bohong, et al. “**[Multi-Classes and Motion Properties for Concurrent Visual SLAM in Dynamic Environments.](https://doi.org/10.1109/TMM.2021.3110667)**” *IEEE Transactions on Multimedia*, 2021

- Yang Gengshan and Ramanan Deva. “**[Learning to Segment Rigid Motions from Two Frames.](http://arxiv.org/abs/2101.03694)**” CVPR 2021

  - [Project page](https://www.contrib.andrew.cmu.edu/~gengshay/cvpr21rigidmask.html).

- Thomas Hugues, et al. “**[Learning Spatiotemporal Occupancy Grid Maps for Lifelong Navigation in Dynamic Scenes.](http://arxiv.org/abs/2108.10585)**” 

  - [code](https://github.com/utiasASRL/Deep-Collison-Checker).

- Jung Dongki, et al. “**[DnD: Dense Depth Estimation in Crowded Dynamic Indoor Scenes.](http://arxiv.org/abs/2108.05615)**” (ICCV 2021)

  - code, video.
  
- Luiten Jonathon, et al. “[**Track to Reconstruct and Reconstruct to Track.**](https://arxiv.org/abs/1910.00130v3)”, (RAL+ICRA 2020)

  - [code](https://github.com/tobiasfshr/MOTSFusion), [video](https://youtu.be/PMOYkpBwE78). **Reconstruct**.

- Grinvald, Margarita, et al. “**[TSDF++: A Multi-Object Formulation for Dynamic Object Tracking and Reconstruction.](http://arxiv.org/abs/2105.07468)**”(ICRA 2021)

  - [code](https://github.com/ethz-asl/tsdf-plusplus), [video](https://youtu.be/dSJmoeVasI0).

- **Wang Chieh-Chih, et al. “[Simultaneous Localization, Mapping and Moving Object Tracking.](https://www.ri.cmu.edu/pub_files/pub4/wang_chieh_chih_2007_1/wang_chieh_chih_2007_1.pdf)” *The International Journal of Robotics Research 2007***

- Ran Teng, et al. “**[RS-SLAM: A Robust Semantic SLAM in Dynamic Environments Based on RGB-D Sensor](https://doi.org/10.1109/JSEN.2021.3099511)**.” 

- Xu Hua, et al. “OD-SLAM: Real-Time Localization and Mapping in Dynamic Environment through Multi-Sensor Fusion.” * (ICARM 2020)* https://doi.org/10.1109/ICARM49381.2020.9195374.

- Wimbauer Felix, et al. “**[MonoRec: Semi-Supervised Dense Reconstruction in Dynamic Environments from a Single Moving Camera.](http://arxiv.org/abs/2011.11814)**” (CVPR 2021)

  - **[Project page](https://vision.in.tum.de/research/monorec)**. [code](https://github.com/Brummi/MonoRec). [video](https://youtu.be/-gDSBIm0vgk). [video 2](https://youtu.be/-gDSBIm0vgk).

- Liu Yu, et al. “Dynamic RGB-D SLAM Based on Static Probability and Observation Number.” *IEEE Transactions on Instrumentation and Measurement*, vol. 70, 2021, pp. 1–11. *IEEE Xplore*, https://doi.org/10.1109/TIM.2021.3089228.

- P. Li, T. Qin, and S. Shen, “**[Stereo Vision-based Semantic 3D Object and Ego-motion Tracking for Autonomous Driving](http://arxiv.org/abs/1807.02062)**,” arXiv 2018

  - 沈邵颉老师组

- G. B. Nair *et al.*, “**[Multi-object Monocular SLAM for Dynamic Environments](http://arxiv.org/abs/2002.03528)**,” IV2020

- M. Rünz and L. Agapito, “[**Co-fusion: Real-time segmentation, tracking and fusion of multiple objects,**](https://doi.org/10.1109/ICRA.2017.7989518)” in *2017 IEEE International Conference on Robotics and Automation (ICRA)*, May 2017, pp. 4471–4478.

  - [code](https://github.com/martinruenz/co-fusion), 

- [TwistSLAM: Constrained SLAM in Dynamic Environment](https://arxiv.org/pdf/2202.12384),
  - S3LAM的后续，使用全景分割作为检测的前端


# Object SLAM & Application

- **CubeSLAM: Monocular 3D Object SLAM**, IEEE Transactions on Robotics 2019, S. Yang, S. Scherer [**PDF**](https://arxiv.org/abs/1806.00557)
  - [code](https://github.com/shichaoy/cube_slam). [video](https://youtu.be/QnVlexXi9_c). Vision
- Salas-Moreno Renato F., et al. “**[SLAM++: Simultaneous Localisation and Mapping at the Level of Objects.](https://doi.org/10/ggmwnd)**” (CVPR 2013)
  - code, [video](https://youtu.be/tmrAh1CqCRo),
- Nicholson Lachlan, et al. “**[QuadricSLAM: Dual Quadrics From Object Detections as Landmarks in Object-Oriented SLAM](https://arxiv.org/abs/1804.04011)**.” (RAL-2018)
  - [**Project page**](https://nikosuenderhauf.github.io/semanticslam.ai/quadricslam.html), [code](https://github.com/tiev-tongji/quadric_slam-deprecated).
- Wu Yanmin, et al. “[**EAO-SLAM: Monocular Semi-Dense Object SLAM Based on Ensemble Data Association**](https://arxiv.org/abs/2004.12730).” *2020 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*, Oct. 2020, pp. 4966–73. *arXiv.org*, https://doi.org/10.1109/IROS45743.2020.9341757.
  - [Project page](https://yanmin-wu.github.io/project/eaoslam/). [code](https://github.com/yanmin-wu/EAO-SLAM).  
- H. Osman, N. Darwish, and A. Bayoumi, “LoopNet: Where to Focus Detecting Loop Closures in Dynamic Scenes,” *IEEE Robotics and Automation Letters*, pp. 1–1, 2022, doi: [10.1109/LRA.2022.3142901](https://doi.org/10.1109/LRA.2022.3142901).
  - 动态环境中的回环检测，网络。code，video

- M. N. Finean, L. Petrović, W. Merkt, I. Marković, and I. Havoutis, “**[Motion Planning in Dynamic Environments Using Context-Aware Human Trajectory Prediction](http://arxiv.org/abs/2201.05058)**,” *arXiv:2201.05058 [cs]*, Jan. 2022.
  - 含有人的动态环境的导航，**[code](https://github.com/ori-drs/integrated-dynamic-motion-planning-framework)**，**[video](https://www.youtube.com/watch?v=gdC3mpZNjG4&t=5s)**。类似避障和规划类的


# Researchers

## 🥼1. Berta Bescos

> **主页：[谷歌学术](https://scholar.google.hk/citations?user=8koVpHwAAAAJ&hl=it) | [个人主页](https://bertabescos.github.io/) | [GitHub](https://github.com/BertaBescos)**

> **博士学位论文： [Visual slam in dynamic environments](https://zaguan.unizar.es/record/100672)**

> **Contributions**

- 【检测】第一部分的目标是**使动态物体的检测成为一个独立的或在视觉 SLAM 框架内的模块**。对于后者我们的目标是最小化相机轨迹估计的误差，并减少创建的地图中错误和不稳定数据的存在，这是在现实环境中长期应用的必要条件。我们提出了一种新方法，**利用深度学习中的语义分割和多视图几何方法来检测先验动态和移动物体**。实验表明，可以在高动态场景中实现与静态环境中实现的 SLAM 精度相当的精度，并且可以**构建仅包含静态和稳定环境结构的三维地图**。尽管机器人界普遍认为动态是根据语义类别来定义的，但我们证明可以通过自监督的方式获得这些知识。[文献 **1**]
- 【图像修复】第二部分解决了**原图像中动态物体剔除之后的图像修复问题**。总体目标是**在动态环境中改进基于视觉的定位和建图任务**，其中在不同时刻不同动态物体的存在或不存在会使这些任务的鲁棒性降低。我们**提出了一种数据驱动的方法来获取动态场景的静态图像，抠除使用相机扫描场景时可能存在的动态物体**。为了实现这一目标，我们引入了端到端的深度学习框架，**将包含动态内容（例如车辆或行人）的城市环境图像转换为适合定位和建图的逼真的静态图像**。这是通过**生成对抗模型**来实现的，该模型将原始动态图像及其动态/静态二进制掩码作为输入，能够生成最终的静态图像。该框架利用了两种新的损失，一种基于图像隐写分析技术，有助于提高修复质量，另一种基于 ORB 特征，旨在增强真实和幻觉图像区域之间的特征匹配。[文献 **2, 3**]
- 【多目标跟踪】最后一部分**不仅关注于实现鲁棒的相机跟踪和稳定的地图构建，还关注于跟踪场景中存在的所有动态目标的姿势**。目标是通过最小化相机轨迹估计和周围智能体的误差，为 SLAM 和多目标跟踪开发一个联合框架。因此，我们提出了一个基于特征的 SLAM 框架，适配双目和 RGB-D 相机，其前端和后端为**多目标跟踪**量身定制。鉴于目标跟踪增加了 SLAM 问题的复杂性，我们通过特别关注所涉及的参数数量来解决该问题，以保持实时性能。我们证明，这两项任务彼此非常有益，与当前文献中的常用方法相矛盾。为了验证这种方法，我们对室内外多种环境中的**自运动和目标跟踪**进行了广泛的评估，证明在**不假设场景先验**的情况下获得最先进的性能是可能的。[文献 **4**]

> **代表性工作**

- **[1]** Bescos B, Fácil J M, Civera J, et al. [DynaSLAM: Tracking, mapping, and inpainting in dynamic scenes](https://arxiv.org/pdf/1806.05620.pdf)[J]. IEEE Robotics and Automation Letters, **2018**, 3(4): 4076-4083.
- **[2]** Bescos B, Neira J, Siegwart R, et al. [Empty cities: Image inpainting for a dynamic-object-invariant space](https://arxiv.org/pdf/1809.10239.pdf)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 5460-5466.
- **[3]** Bescos B, Cadena C, Neira J. [Empty cities: A dynamic-object-invariant space for visual SLAM](https://arxiv.org/pdf/2010.07646.pdf)[J]. IEEE Transactions on Robotics, **2020**, 37(2): 433-451.
- **[4]** Bescos B, Campos C, Tardós J D, et al. [DynaSLAM II: Tightly-coupled multi-object tracking and SLAM](https://arxiv.org/pdf/2010.07820.pdf)[J]. IEEE Robotics and Automation Letters, **2021**, 6(3): 5191-5198.

## 🥼2. Yubao Liu

[Walk Into AI World](https://www.ybliu.com/)

> 主页：[谷歌学术](https://scholar.google.com/citations?user=P4M6ru0AAAAJ&hl=zh-CN) | [GitHub](https://github.com/yubaoliu)

> 代表性工作：

1. RDS-SLAM: real-time dynamic SLAM using semantic segmentation methods
2. KMOP-vSLAM: Dynamic Visual SLAM for RGB-D Cameras using K-means and OpenPose
3. RDMO-SLAM: Real-time Visual SLAM for Dynamic Environments using Semantic Label Prediction with Optical Flow
