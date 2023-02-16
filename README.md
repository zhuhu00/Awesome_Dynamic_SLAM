# Awesome_Dynamic_SLAM [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

The following paper are the papers that focuses on the **SLAM in dynamic Environments** and **Life-long SLAM**. In the dynamic environment, there are two kinds of robust SLAM: First is **detection & removal**. Another is **detection & tracking**. Although the mapping part in dynamic environment is not my focus, but I will also put some articles yet also very interesting.

> **Vision** means that the pipeline is built with camera. Others are the same, such as **lidar**, **radar**, **sensor fusion**.

------

# Related survey papers:

- [**A survey: which features are required for dynamic visual simultaneous localization and mapping?**](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8285453/pdf/42492_2021_Article_86.pdf). Zewen Xu,CAS. 2021

- [**State of the Art in Real-time Registration of RGB-D Images**](https://cg.cs.uni-bonn.de/aigaion2root/attachments/StateoftheArtinReal-timeRegistrationofRGB-DImages.pdf). Stotko, Patrick. University of Bonn. 2016
- [**Visual SLAM and Structure from Motion in Dynamic Environments: A Survey**](https://dl.acm.org/doi/pdf/10.1145/3177853).  University of Oxford. 2018
- [**State of the Art on 3D Reconstruction with RGB-D Cameras**](https://www.cg.informatik.uni-siegen.de/data/Publications/2018/star1009-main.pdf). Michael Zollhöfer. Stanford University. 2018

# Dynamic Object Detection and *Removal*

- (IROS 2022)[CFP-SLAM: A Real-time Visual SLAM Based on Coarse-to-Fine Probability in Dynamic Environments](https://arxiv.org/pdf/2202.01938v2.pdf)

- (IROS 2022) [DRG-SLAM: A Semantic RGB-D SLAM using Geometric Features for Indoor Dynamic Scene](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9981238)

- (IEEE RA-L'22)[DynaVINS: A Visual-Inertial SLAM for Dynamic Environments](https://arxiv.org/pdf/2208.11500), code:https://github.com/url-kaist/dynaVINS, 非深度学习结合的方案，而是使用约束对运动对象上的特征点进行去除

- [DeFlowSLAM: Self-Supervised Scene Motion Decomposition for Dynamic Dense  SLAM](https://arxiv.org/pdf/2207.08794v1)
  
  - 浙江大学，貌似是DROID-SLAM得部分，将光流分成了动态物体和静态，分别进行后续的操作。效果看起来也很不错。[page](https://zju3dv.github.io/deflowslam/)，[code](https://github.com/zju3dv/DeFlowSLAM)
  
- [Efficient Spatial-Temporal Information Fusion for LiDAR-Based 3D Moving  Object Segmentation](https://arxiv.org/pdf/2207.02201)

  - 毫末智行，**[code](https://github.com/haomo-ai/MotionSeg3D)**，动态检测

- [[2203.03923] ROLL: Long-Term Robust LiDAR-based Localization With Temporary Mapping in Changing Environments](https://arxiv.org/pdf/2203.03923) IROS 2022

  - code：https://github.com/HaisenbergPeng/ROLL

- [POCD: Probabilistic Object-Level Change Detection and Volumetric Mapping  in Semi-Static Scenes](https://arxiv.org/pdf/2205.01202v1)

  - RSS 2022，半静态场景中的地图更新

- J. Schauer and A. Nuchter, “**The Peopleremover—Removing Dynamic Objects From 3-D Point Cloud Data by Traversing a Voxel Occupancy Grid**,” *IEEE Robot. Autom. Lett.*, vol. 3, no. 3, pp. 1679–1686, Jul. 2018, doi: [10.1109/LRA.2018.2801797](https://doi.org/10.1109/LRA.2018.2801797).

  - 基于体素遍历的方法的运动对象去除，虽然这种方法有很多的缺点，但是论文提出了很多的trick，来解决这些问题，看起来效果还是不错的。
  - code，video

- N. Rufus, U. K. R. Nair, A. V. S. S. B. Kumar, V. Madiraju, and K. M. Krishna, “[**SROM: Simple Real-time Odometry and Mapping using LiDAR data for Autonomous Vehicles**.](http://arxiv.org/abs/2005.02042)” IV 2020
  - 较为粗暴的去除可能的运动对象，去除地面后再取出

- M. Schorghuber, D. Steininger, Y. Cabon, M. Humenberger, and M. Gelautz, “**[SLAMANTIC - Leveraging Semantics to Improve VSLAM in Dynamic Environments,](https://openaccess.thecvf.com/content_ICCVW_2019/papers/DL4VSLAM/Schorghuber_SLAMANTIC_-_Leveraging_Semantics_to_Improve_VSLAM_in_Dynamic_Environments_ICCVW_2019_paper.pdf)**” ICCV 2019 workshop
  - 视觉SLAM，动态环境。通过语义对点的置信度进行计算，高置信度的点来辅助低置信度的点，最终确定用于定位和建图的部分。

- S. Gu, S. Yao, J. Yang, and H. Kong, “**[Semantics-Guided Moving Object Segmentation with 3D LiDAR]( http://arxiv.org/abs/2205.03186)**,”  arxiv 2022.05
  - 动态物体的分割网络，也是rangenet的思想那套。

- Y. Pan, B. Gao, J. Mei, S. Geng, C. Li, and H. Zhao, “**[SemanticPOSS: A Point Cloud Dataset with Large Quantity of Dynamic Instances](https://arxiv.org/pdf/2002.09147v1.pdf)**,” IV 2020
  - 动态物体室外数据集，北大，[网站](http://www.poss.pku.edu.cn/semanticposs.html)

- S. Pagad, D. Agarwal, S. Narayanan, K. Rangan, H. Kim, and G. Yalla, “**[Robust Method for Removing Dynamic Objects from Point Clouds](https://drive.google.com/file/d/1o73aG85OpuDmAUsjkgKaVwrG6d48aOin/view)**,” ICRA 2020
  - [video](https://www.youtube.com/watch?v=d2rbSP9IkkY)，动态去除

- L. Sun, Z. Yan, A. Zaganidis, C. Zhao, and T. Duckett, “**Recurrent-OctoMap: Learning State-Based Map Refinement for Long-Term Semantic Mapping With 3-D-Lidar Data**,” RAL
  - life long slam 

- P. Egger, P. V. K. Borges, G. Catt, A. Pfrunder, R. Siegwart, and R. Dubé, “**PoseMap: Lifelong, Multi-Environment 3D LiDAR Localization**,” IROS 2018
  - lifelong slam，ETH SAL组

- DynamicFilter: **an Online Dynamic Objects Removal Framework for Highly Dynamic Environments**，ICRA 2022
  - IJRR大佬，可惜不开源。。，港大，南科大

- X. Ma, Y. Wang, B. Zhang, H.-J. Ma, and C. Luo, “**[DynPL-SVO: A New Method Using Point and Line Features for Stereo Visual Odometry in Dynamic Scenes](https://arxiv.org/abs/2205.08207v1)**.” arXiv, May 17, 2022
  - 使用点和线特征的双目视觉里程计，动态去除的论文
  - 东北大学，也还没有开源

- M. T. Lázaro, R. Capobianco, and G. Grisetti, “**[Efficient Long-term Mapping in Dynamic Environments](https://www.researchgate.net/profile/Maria-Lazaro-12/publication/330586668_Efficient_Long-term_Mapping_in_Dynamic_Environments/links/5f26efbe458515b729fe2f1b/Efficient-Long-term-Mapping-in-Dynamic-Environments.pdf)**,” IROS 2018
  - 高效的ICP方案，并且实现了地图实体的合并。由于处理的是2D地图，因此也就没有那么多的需要处理的东西。可以直接用点可视化来去除运动的点云。
  - **[code](https://gitlab.com/srrg-software/srrg_mapper2d_ros)**，

- T. Krajník, J. P. Fentanes, J. M. Santos, and T. Duckett, “**[FreMEn: Frequency Map Enhancement for Long-Term Mobile Robot Autonomy in Changing Environments](http://strands.acin.tuwien.ac.at/publications/y4/krajnik_TRO.pdf)**,” TRO 2017

- G. Kurz, M. Holoch, and P. Biber, “[**Geometry-based Graph Pruning for Lifelong SLAM**](http://arxiv.org/abs/2110.01286).” IROS 2021
  - 我们提出了一种新的方法，该方法考虑了几何准则来选择要剪枝的顶点。这是有效的，易于实现，并导致具有均匀分布的顶点的图形，这些顶点仍然是机器人轨迹的一部分。此外，我们提出了一种新的边际化方法，与现有方法相比，该方法对错误的循环闭包具有更强的鲁棒性。
    主要设计到SLAM后端的优化，当地图或者是因子图更新时，如何对因子图进行剪枝的问题。

- Quei-An Chen and Akihiro Tsukada，“[**Flow Supervised Neural Radiance Fields for Static-Dynamic Decomposition**](https://drive.google.com/file/d/1kORAX0DOAs7m771EQ693aH7FeRwUqhCy/view)”, ICRA 2022
  - AI葵，[**code**](https://github.com/kwea123?tab=repositories)，nerf+光流的动态物体，去除并修复，[video](https://youtu.be/ixw9AkJpe30)。

- W. Ding, S. Hou, H. Gao, G. Wan, and S. Song, “[**LiDAR Inertial Odometry Aided Robust LiDAR Localization System in Changing City Scenes**](https://songshiyu01.github.io/pdf/LIO_W.Ding_S.Song_ICRA2020.pdf),” ICRA 2020
  - 百度出品的使用激光和IMU，在运动场景的定位，并且在之前构建的地图中，针对场景新增加的东西，将会新建相关的地图。
  - life-long SLAM

- G. D. Tipaldi, D. Meyer-Delius, and W. Burgard, “**Lifelong localization in changing environments**,” IJRR 2013
  - life-long的定位

- S. Zhu, X. Zhang, S. Guo, J. Li, and H. Liu, “**Lifelong Localization in Semi-Dynamic Environment**,” ICRA 2021
  - 清华，life-long的定位

- F. Pomerleau, P. Krüsi, F. Colas, P. Furgale, and R. Siegwart, “**Long-term 3D map maintenance in dynamic environments**,” ICRA 2014
  - 动态环境中，地图更新

- D. J. Yoon, T. Y. Tang, and T. D. Barfoot, “[**Mapless Online Detection of Dynamic Objects in 3D Lidar**](http://arxiv.org/abs/1809.06972).” Conference on Computer and Robot Vision (CRV) 2019
  - 点云动态检测

- M. Zhao *et al.*, “[**A General Framework for Lifelong Localization and Mapping in Changing Environment**](http://arxiv.org/abs/2111.10946).”  IROS 2021

  - 高仙机器人的**life-long** 定位的论文
  - 多session的地图表示和一种**高效的在线地图更新策略**，子系统组成：局部激光雷达里程计（LLO）、全局激光雷达匹配（GLM）和位姿图优化（PGR），LLO的作用是构建一系列局部一致的子地图，GLM子系统负责计算传入扫描点云和全局子地图之间的相对约束，并将子映地图和约束插入PGR，PGR是系统中最重要的部分，它从LLO和GLM收集子地图和约束关系，修剪并保存在历史地图中的旧的子地图，并执行姿势图稀疏化和优化。

- D. Henning, T. Laidlow, and S. Leutenegger, “[**BodySLAM: Joint Camera Localisation, Mapping, and Human Motion Tracking**](https://arxiv.org/pdf/2205.02301v1.pdf),” *arXiv:2205.02301

  - 人体构建和SLAM相结合，与AirDOS有点类似

- Pfreundschuh, Patrick, et al. “**[Dynamic Object Aware LiDAR SLAM Based on Automatic Generation of Training Data.](http://arxiv.org/abs/2104.03657)**” (*ICRA* *2021*)

  - **ETH ASL**,code, [video](https://youtu.be/LcDxd97r1Gc), [**dataset**](https://projects.asl.ethz.ch/datasets/doals), Lidar
  - 作者基于deep-learning（3D-MiniNet网络）进行实时3D动态物体检测，滤除动态物体后的点云被喂给LOAM，进行常规的激光SLAM。提供了学习的方法是属于无监督的方法。

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

  1. Liu Yubao and Miura Jun. “RDMO-SLAM: Real-Time Visual SLAM for Dynamic Environments Using Semantic Label Prediction With Optical Flow.” *IEEE Access*, vol. 9, 2021, pp. 106981–97. *IEEE Xplore*, https://doi.org/10.1109/ACCESS.2021.3100426.

  - [code](https://github.com/yubaoliu/RDS-SLAM.git
    ), video.

- Cheng Jiyu, et al. “**Improving Visual Localization Accuracy in Dynamic Environments Based on Dynamic Region Removal.**” *IEEE Transactions on Automation Science and Engineering*, vol. 17, no. 3, July 2020, pp. 1585–96. *IEEE Xplore*, https://doi.org/10.1109/TASE.2020.2964938.

- Soares João Carlos Virgolino, et al. “**[Crowd-SLAM: Visual SLAM Towards Crowded Environments Using Object Detection.](https://doi.org/10.1007/s10846-021-01414-1)**” *Journal of Intelligent & Robotic Systems* 2021

  - [code](https://github.com/virgolinosoares/Crowd-SLAM), video
  - [Visual Localization and Mapping in Dynamic and Changing Environments (2022)](https://arxiv.org/pdf/2209.10710.pdf), 之前的是在orbslam2上，最新的是orbslam3.

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

- (IROS 2022)Dynamic-VINS：RGB-D Inertial Odometry for a Resource-restricted Robot in Dynamic Environments. 
  - 分割+运动点置信度，[code](https://github.com/HITSZ-NRSL/Dynamic-VINS),[video](https://www.bilibili.com/video/BV1bF411t7mx)

# Dynamic Object Detection and ***Tracking***

- [DyOb-SLAM : Dynamic Object Tracking SLAM System (2022)](https://arxiv.org/pdf/2211.01941.pdf)
  - VDO-SLAM+DynaSLAM的结合。。。

- [DynaVIG: Monocular Vision/INS/GNSS Integrated Navigation and Object  Tracking for AGV in Dynamic Scenes (2022)](https://arxiv.org/pdf/2211.14478.pdf)

- [DirectTracker: 3D Multi-Object Tracking Using Direct Image Alignment and  Photometric Bundle Adjustment (2022)](https://arxiv.org/pdf/2209.14965.pdf)
  - 直接法的动态物体追踪，[page](https://vision.in.tum.de/research/vslam/directtracker)

- (IROS 2022)[MOTSLAM: MOT-assisted monocular dynamic SLAM using single-view depth  estimation (2022)](https://arxiv.org/pdf/2210.02038.pdf)
- [TwistSLAM++: Fusing multiple modalities for accurate dynamic semantic  SLAM (2022)](https://arxiv.org/pdf/2209.07888.pdf)
  - SLAMMOT
- (IROS 2022)[Visual-Inertial Multi-Instance Dynamic SLAM with Object-level  Relocalisation (2022)](https://arxiv.org/pdf/2208.04274.pdf)
  - IROS 2022，实验室网址：https://mlr.in.tum.de/research/semanicobjectlevelanddynamicslam
- [Learning to Complete Object Shapes for Object-level Mapping in Dynamic  Scenes (2022)](https://arxiv.org/pdf/2208.05067.pdf)，与上面是同一个作者，
  - 都是基于MID-Fusion做的东西。

- T. Ma and Y. Ou, “[**MLO: Multi-Object Tracking and Lidar Odometry in Dynamic Environment**](http://arxiv.org/abs/2204.11621).” arXiv, Apr. 29, 2022
  - SLAM+MOT了
  
- Z. Wang, W. Li, Y. Shen, and B. Cai, “**[4-D SLAM: An Efficient Dynamic Bayes Network-Based Approach for Dynamic Scene Understanding](https://doi.org/10.1109/ACCESS.2020.3042339)**,” *IEEE Access*
  - 语义识别动态后，使用UKF之类的进行动态追踪，但是图的效果不好。

- T. Ma and Y. Ou, “**[MLO: Multi-Object Tracking and Lidar Odometry in Dynamic Environment](http://arxiv.org/abs/2204.11621)**.” , ArXiv 2022
  - 基于LOAM的目标追踪，分别对运动对象和自身进行估计，之后进行融合。属于松耦合的感觉

- (IROS 2022)R. Long, C. Rauch, T. Zhang, V. Ivan, T. L. Lam, and S. Vijayakumar, “**[RGB-D SLAM in Indoor Planar Environments with Multiple Large Dynamic Objects](http://arxiv.org/abs/2203.02882)**,” 
  - 先做了动态移除，这是动态追踪的。在结构化环境（面）中进行SLAM+MOT

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

- (IROS 2022)[TwistSLAM: Constrained SLAM in Dynamic Environment](https://arxiv.org/pdf/2202.12384),
  - S3LAM的后续，使用全景分割作为检测的前端

# Other Application

- [3D VSG: Long-term Semantic Scene Change Prediction through 3D Variable  Scene Graphs (2022)](https://arxiv.org/pdf/2209.07896.pdf) 
  
  - 语义场景的变化检测
  - code：https://github.com/ethz-asl/3d_vsg

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

- (IROS 2022)[Extrinsic Camera Calibration from A Moving Person](https://vision.ist.i.kyoto-u.ac.jp/pubs/SLee_RAL22.pdf)

- (IROS 2022)[ACEFusion : Accelerated and Energy-Efficient Semantic 3D Reconstruction of Dynamic Scenes](https://pure.manchester.ac.uk/ws/portalfiles/portal/228491926/ACEFusion_IROS2022.pdf)

- (IROS 2022)[Efficient 2D LIDAR-Based Map Updating For Long-Term Operations in Dynamic Environments](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9982047)

- (IROS 2022)[Detecting Invalid Map Merges in Lifelong SLAM](https://arxiv.org/pdf/2211.03423v1.pdf)
- (IROS 2022)[Probabilistic Object Maps for Long-Term Robot Localization](https://arxiv.org/pdf/2110.00128v4.pdf)
- (IROS 2022)[ROLL: Long-Term Robust LiDAR-based Localization With Temporary Mapping in Changing Environments](https://arxiv.org/pdf/2203.03923v1.pdf)
# Researchers
TBD
