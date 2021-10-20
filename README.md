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
  - **ETH ASL**,code, [video](https://youtu.be/LcDxd97r1Gc), [dataset](https://projects.asl.ethz.ch/datasets/doals),
- Canovas Bruce, et al. “[**Speed and Memory Efficient Dense RGB-D SLAM in Dynamic Scenes.**](https://doi.org/10.1109/IROS45743.2020.9341542)” (*IROS* 2020)
  - **GIPSA-lab**, [code](https://github.com/BruceCanovas/supersurfel_fusion), [video](https://youtu.be/hzzVVHUAO74)
- Yuan Xun and Chen Song. “[**SaD-SLAM: A Visual SLAM Based on Semantic and Depth Information.**](http://ras.papercept.net/images/temp/IROS/files/0092.pdf)” *(IROS 2020)*
  - **USTC**, code, video
- Dong, Erqun, et al. “[**Pair-Navi: Peer-to-Peer Indoor Navigation with Mobile Visual SLAM.**](https://cswu.me/papers/infocom19_pairnavi.pdf)” (ICCC 2019)
  - Tsinghua, [Code](https://github.com/Horacehxw/Dynamic_ORB_SLAM2), Video, [Slides](https://slidetodoc.com/pairnavi-peertopeer-indoor-navigation-with-mobile-visual-slam/).

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
- Zhang Jun, et al. “**[VDO-SLAM: A Visual Dynamic Object-Aware SLAM System](http://arxiv.org/abs/2005.11052)**.” (ArXiv 2020)
  - [code](https://github.com/halajun/vdo_slam), video, Vision







# Object SLAM(Data Association)

- **CubeSLAM: Monocular 3D Object SLAM**, IEEE Transactions on Robotics 2019, S. Yang, S. Scherer [**PDF**](https://arxiv.org/abs/1806.00557)
  - [code](https://github.com/shichaoy/cube_slam). [video](https://youtu.be/QnVlexXi9_c). Vision

