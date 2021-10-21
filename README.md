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
- Chen Xieyuanli, et al. “Moving Object Segmentation in 3D LiDAR Data: A Learning-Based Approach Exploiting Sequential Data.” *IEEE Robotics and Automation Letters*, 2021, pp. 1–1. *DOI.org (Crossref)*, https://doi.org/10.1109/LRA.2021.3093567.
  - [code](https://github.com/PRBonn/LiDAR-MOS). [video](https://www.youtube.com/watch?v=NHvsYhk4dhw). University of Bonn.
- Zhang Tianwei, et al. “[**FlowFusion: Dynamic Dense RGB-D SLAM Based on Optical Flow.**](http://arxiv.org/abs/2003.05102.)”(ICRA 2020)
  - code. [video](https://youtu.be/6yPGDdwKFLA).
- Zhang Tianwei, et al. “**[AcousticFusion: Fusing Sound Source Localization to Visual SLAM in Dynamic Environments.](http://arxiv.org/abs/2108.01246)**”,IROS 2021
  - [video](https://youtu.be/8eNikzp9LIQ). 

# Dynamic Object Detection and ***Tracking***

- “**[AirDOS: Dynamic SLAM benefits from Articulated Objects,](http://arxiv.org/abs/2109.09903)**” Qiu Yuheng, et al. 2021(Arxiv)
  - [code](https://github.com/haleqiu/airdos)(TBA), [Paper](https://arxiv.org/abs/2109.09903), Video. **CMU RI**, Vision.
  
- “[**DOT: Dynamic Object Tracking for Visual SLAM**](http://arxiv.org/abs/2010.00052).” Ballester, Irene, et al.(ICRA 2021)
  - code, [video](https://youtu.be/9hWChyQGKJk), **University of Zaragoza**, Vision
  
- Liu Yubao and Miura Jun. “[**RDMO-SLAM: Real-Time Visual SLAM for Dynamic Environments Using Semantic Label Prediction With Optical Flow**](https://doi.org/10.1109/ACCESS.2021.3100426).” *IEEE Access*. 

- Kim Aleksandr, et al. “[**EagerMOT: 3D Multi-Object Tracking via Sensor Fusion.**](http://arxiv.org/abs/2104.14682)” (*ICRA 2021*)
  - **TUM**, [code](https://github.com/aleksandrkim61/EagerMOT), [video](https://youtu.be/k8pKpvbenoM), Sensor Fusion.
  
- Vincent, Jonathan, et al. “[**Dynamic Object Tracking and Masking for Visual SLAM.**](https://arxiv.org/abs/2008.00072v1)” (IROS 2021)
  - code, video, Vision
  
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

  - code, video, 

- Huang, Jiahui, et al. “**[ClusterVO: Clustering Moving Instances and Estimating Visual Odometry for Self and Surroundings](http://arxiv.org/abs/2003.12980)**.” (CVPR 2020)

  - Tsinghua, code, [video](https://youtu.be/paK-WCQpX-Y).[slides](https://cg.cs.tsinghua.edu.cn/people/~huangjh/clustervo-slides.pdf).

- Liu, Yuzhen, et al. “**[A Switching-Coupled Backend for Simultaneous Localization and Dynamic Object Tracking.](https://github.com/zhuhu00/Awesome_Dynamic_SLAM/tree/main/pdfs/liu_2021_SwitchingCoupled.pdf)**” (RAL 2021)

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

# Object SLAM(Data Association)

- **CubeSLAM: Monocular 3D Object SLAM**, IEEE Transactions on Robotics 2019, S. Yang, S. Scherer [**PDF**](https://arxiv.org/abs/1806.00557)
  - [code](https://github.com/shichaoy/cube_slam). [video](https://youtu.be/QnVlexXi9_c). Vision
- Salas-Moreno Renato F., et al. “**[SLAM++: Simultaneous Localisation and Mapping at the Level of Objects.](https://doi.org/10/ggmwnd)**” (CVPR 2013)
  - code, [video](https://youtu.be/tmrAh1CqCRo),
- Nicholson Lachlan, et al. “**[QuadricSLAM: Dual Quadrics From Object Detections as Landmarks in Object-Oriented SLAM](https://arxiv.org/abs/1804.04011)**.” (RAL-2018)
  - [**Project page**](https://nikosuenderhauf.github.io/semanticslam.ai/quadricslam.html),[code](https://github.com/tiev-tongji/quadric_slam-deprecated).
- Wu Yanmin, et al. “[**EAO-SLAM: Monocular Semi-Dense Object SLAM Based on Ensemble Data Association**](https://arxiv.org/abs/2004.12730).” *2020 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*, Oct. 2020, pp. 4966–73. *arXiv.org*, https://doi.org/10.1109/IROS45743.2020.9341757.
  - [Project page](https://yanmin-wu.github.io/project/eaoslam/). [code](https://github.com/yanmin-wu/EAO-SLAM).  

# Researchers

1. 
