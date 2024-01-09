<h1 align="center">Awesome 3D Face Reconstruction (Kor.)</h1>
<p align="center"><a href="https://github.com/winterbloooom/awesome-3d-face-reconstruction"><img src="https://awesome.re/badge.svg"></a></p>

<details>
  <summary>🪄 <b>Table of Contents</b></summary>

  - [3D Face Reconstruction](#3d-face-reconstruction)
    - 📑 [Papers](#-papers)
    - 🫥 [Facial/Head Models](#-facialhead-models)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks)
    - 📦 [Datasets](#-datasets)
  - [Face Animation with Audio (Talking Head)](#face-animation-with-audio-talking-head)
    - 📑 [Papers](#-papers-1)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks-1)
    - 📦 [Datasets](#-datasets-1)
</details>

<details>
<summary>Conference/Journal Name Abbr.</summary>

| Abbr. | Full name |
|-------|-----------|
|AVSS       | International Conference on Advanced Video and Signal Based Surveillance |
|CVPR       ||
|ICCV       | International Conference on Computer Vision |
|ToG        ||
|SIGGRAPH   ||
|FG         | IEEE International Conference on Automatic Face & Gesture Recognition|
|TVCG       | IEEE Transactions on Visualization and Computer Graphics|
|TAG        | IEEE Transactions on Affective Computing|
|PR         | Pattern Recognition |
|TMM        | IEEE Transactions on Multimedia |
|MM         | ACM Multimedia Conference |
|TIP        | IEEE Transactions on Image Processing |
|J-HGBU     | Joint ACM Workshop on Human Gesture and Behavior Understanding |
</details>

> [!NOTE]
> - 논문은 **발표 연도 역순**으로 정렬되었으며, arXiv에 선공개 되었어도 이후 학회/저널에 발표되었으면 그것을 기준으로 합니다.
> - 중요한 논문은 ✨ 표시했습니다.

## 3D Face Reconstruction
### 📑 Papers

- **[AlbedoGAN](https://aashishrai3799.github.io/Towards-Realistic-Generative-3D-Face-Models/)** (2024 WACV) [[Code](https://github.com/aashishrai3799/Towards-Realistic-Generative-3D-Face-Models/)]<br>
**Towards Realistic Generative 3D Face Models**<br>
*Aashish Rai, Hiresh Gupta, Ayush Pandey, Francisco Vicente Carrasco, Shingo Jason Takagi, Amaury Aubel, Daeil Kim, Aayush Prakash, Fernando de la Torre*<br>


- **[TokenFace](https://openaccess.thecvf.com/content/ICCV2023/html/Zhang_Accurate_3D_Face_Reconstruction_with_Facial_Component_Tokens_ICCV_2023_paper.html)** (2023 ICCV)<br>
**Accurate 3D Face Reconstruction with Facial Component Tokens**<br>
*Tianke Zhang, Xuangeng Chu, Yunfei Liu, Lijian Lin, Zhendong Yang, Zhengzhuo Xu, Chengkun Cao, Fei Yu, Changyin Zhou, Chun Yuan, Yu Li*<br>
FLAME의 각 파라미터를 decoupling하고자, ViT에 이미지 토큰과 더불어 파라미터를 각각 token으로 만들어 입력함. 2&3D dataset을 동시에 사용함.


- **[HiFace](https://project-hiface.github.io/)** (2023 ICCV)<br>
**HiFace: High-Fidelity 3D Face Reconstruction by Learning Static and Dynamic Details**<br>
*Zenghao Chai, Tianke Zhang, Tianyu He, Xu Tan, Tadas  Baltrušaitis, HsiangTao Wu, Runnan Li, Sheng Zhao, Chun Yuan, Jiang Bian*<br>
Detail을 static detail과 dynamic detail로 나눔. Synthetic dataset을 사용하여 학습.


- **[FOCUS](https://arxiv.org/abs/2106.09614)** (2023 CVPR) [[Code](https://github.com/unibas-gravis/Occlusion-Robust-MoFA)]<br>
**Robust Model-based Face Reconstruction through Weakly-Supervised Outlier Segmentation**<br>
*Chunlu Li, Andreas Morel-Forster, Thomas Vetter, Bernhard Egger, and Adam Kortylewski*<br>
Reconstruction과 outlier segmentation을 동시에 수행하여 outlier에도 robust한 결과를 얻고자 함.


- **[HRN](https://younglbw.github.io/HRN-homepage/)** (2023 CVPR) [[Code](https://github.com/youngLBW/HRN)]<br>
**A Hierarchical Representation Network for Accurate and Detailed Face Reconstruction from In-The-Wild Images**<br>
*Biwen Lei, Jianqiang Ren, Mengyang Feng, Miaomiao Cui, Xuansong Xie*<br>


- **[DenseLandmarks](https://microsoft.github.io/DenseLandmarks/)** (2022 ECCV)<br>
**3D Face Reconstruction with Dense Landmarks**<br>
*Erroll Wood, Tadas Baltrušaitis, Charlie Hewitt, Matthew Johnson, Jingjing Shen, Nikola Milosavljevic, Daniel Wilde, Stephan Garbin, Chirag Raman, Jamie Shotton, Toby Sharp, Ivan Stojiljkovic, Thomas J. Cashman, Julien Valentin*<br>
700개 이상의 dense landmarks를 uncertainty와 함께 예측함. Synthetic dataset를 사용해 정확한 annotation을 얻을 수 있었음.


- **[MICA](https://zielon.github.io/mica/)** (2022 ECCV) [[Code](https://github.com/Zielon/MICA)]<br>
**Towards Metrical Reconstruction of Human Faces**<br>
*Wojciech Zielonka, Timo Balkart, Justus Thies*<br>
Metrical한 reconstruction을 수행함. Pre-trained face reconstruction model에서 추출한 feature를 사용함으로써 서로 다른 얼굴에 대한 구분성을 높임. 여러 데이터셋을 합쳐 3D dataset을 구축해 supervised learning을 함.


- **[EMOCA](https://emoca.is.tue.mpg.de/)** (2022 CVPR) ✨ [[Code](https://github.com/radekd91/emoca)]<br>
**EMOCA: Emotion Driven Monocular Face Capture and Animation**<br>
*Radek Danecek, Michael Black, Timo Bolkart*<br>
Expression encoder를 추가로 사용함과 동시에, 입력 이미지와 reconstruction 사이의 emotion 차이로 loss를 부여함으로써, emotion이 잘 보존된 결과를 얻음.


- **[SynergyNet](https://arxiv.org/pdf/2110.09772.pdf)** (2021 3DV) [[Code](https://github.com/choyingw/SynergyNet)]<br>
**Synergy between 3DMM and 3D Landmarks for Accurate 3D Facial Geometry**<br>
*Cho-Ying Wu, Qiangeng Xu, Ulrich Neumann*<br>


- **[Dib et al.](https://arxiv.org/pdf/2103.15432.pdf)** (2021 ICCV)<br>
**Towards high fidelity monocular face reconstruction with rich reflectance using self-supervised learning and ray tracing**<br>
*Abdallah Dib, Cedric Thebault, Junghyun Ahn, Philippe-Henri Gosselin, Christian Theobalt, Louis Chevallier*<br>


- **[Fast-GANFIT](https://arxiv.org/abs/2105.07474)** (2021 TPAMI) [[Code](https://github.com/barisgecer/GANFit)]<br>
**Fast-GANFIT: Generative Adversarial Network for High Fidelity 3D Face Reconstruction**<br>
*Baris Gecer, Stylianos Ploumpis, Irene Kotsia, Stefanos Zafeiriou*<br>


- **[DECA](https://arxiv.org/pdf/2012.04012.pdf)** (2021 SIGGRAPH) ✨ [[Code](https://github.com/YadiraF/DECA)]<br>
**Learning an Animatable Detailed 3D Face Model from In-the-Wild Images**<br>
*Yao Feng, Haiwen Feng, Michael J. Black, Timo Bolkart*<br>
Detail을 displacement map으로 예측해 coarse shape에 합쳐 reconstruction을 구성하며, 이로써 다른 이미지의 expression에서 얻은 displacement map으로 교체도 가능. 이후 수많은 모델의 기본 모델로 사용됨.


- **[3DDFA-V2](https://arxiv.org/pdf/2009.09960.pdf)** (2020 ECCV) [[Code](https://github.com/cleardusk/3DDFA_V2)]<br>
**Towards Fast, Accurate and Stable 3D Dense Face Alignment**<br>
*Jianzhu Guo, Xiangyu Zhu, Yang Yang, Fan Yang, Zhen Lei, Stan Z. Li*<br>


- **[MGCNet](https://arxiv.org/pdf/2007.12494.pdf)** (2020 ECCV) [[Code](https://github.com/jiaxiangshang/MGCNet)]<br>
**Self-Supervised Monocular 3D Face Reconstruction by Occlusion-Aware Multi-view Geometry Consistency**<br>
*Jiaxiang Shang, Tianwei Shen, Shiwei Li, Lei Zhou, Mingmin Zhen, Tian Fang, Long Quan*<br>


- **[UMDFA](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123470681.pdf)** (2020 ECCV)<br>
**“Look Ma, no landmarks!” – Unsupervised, model-based dense face alignment**<br>
*Tatsuro Koizumi, William A. P. Smith*<br>


- **[GANFIT](https://arxiv.org/pdf/1902.05978.pdf)** (2019 CVPR) [[Code](https://github.com/barisgecer/GANFit)]<br>
**GANFIT: Generative Adversarial Network Fitting for High Fidelity 3D Face Reconstruction**<br>
*Baris Gecer, Stylianos Ploumpis, Irene Kotsia, Stefanos Zafeiriou*<br>


- **[Luan Tran et al.](https://arxiv.org/abs/1904.04933)** (2019 CVPR) [[Code](https://github.com/tranluan/Nonlinear_Face_3DMM)]<br>
**Towards High-Fidelity Nonlinear 3D Face Morphable Model**<br>
*Luan Tran, Feng Liu, Xiaoming Liu*<br>


- **[RingNet, NoW](https://arxiv.org/pdf/1905.06817.pdf)** (2019 CVPR) ✨ [[Code](https://github.com/soubhiksanyal/RingNet)]<br>
**Learning to Regress 3D Face Shape and Expression from an Image without 3D Supervision**<br>
*Soubhik Sanyal, Timo Bolkart, Haiwen Feng and Michael J. Black*<br>
같은 사람의 사진 간에는 shape consistency를 높이고, 서로 다른 사람의 사진 간에는 shape inconsistency를 낮추도록 학습. 현재 가장 흔히 사용되는 NoW benchmark를 제시함.


- **[Deep3DFaceRecon](https://arxiv.org/abs/1903.08527)** (2019 CVPRw) [[Code](https://github.com/microsoft/Deep3DFaceReconstruction)]<br>
**Accurate 3D Face Reconstruction with Weakly-Supervised Learing: From Single Image to Image Set**<br>
*Yu Deng, Jiaolong Yang, Sicheng Xu, Dong Chen, Yunde Jia, Xin Tong*<br>
GT 없이도 landmark나 facial mask 등으로 self-supervised learning 수행. Confidence measurement subnetwork를 추가로 두어 multi-image reconstruction을 학습.


- **[PRNet](https://arxiv.org/pdf/1803.07835.pdf)** (2018 ECCV) [[Code](https://github.com/YadiraF/PRNet)]<br>
**Joint 3D Face Reconstruction and Dense Alignment with Position Map Regression Network**<br>
*Yao Feng, Fan Wu, Xiaohu Shao, Yanfeng Wang, and Xi Zhou*<br>


- **[Anh Tuấn Trần et al.](https://openaccess.thecvf.com/content_cvpr_2018/html/Tran_Extreme_3D_Face_CVPR_2018_paper.html)** (2018 CVPR) [[Code](https://github.com/anhttran/extreme_3d_faces)]<br>
**Extreme 3D Face Reconstruction: Seeing Through Occlusions**<br>
*Anh Tuấn Trần, Tal Hassner, Iacopo Masi, Eran Paz, Yuval Nirkin, Gérard Medioni*<br>


- **[Ayush Tewari et al.](https://vcai.mpi-inf.mpg.de/projects/FML/)** (2018 CVPR)<br>
**Self-supervised multi-level face model learning for monocular reconstruction at over 250 Hz**<br>
*Ayush Tewari, Michael Zollhöfer, Pablo Garrido, Florian Bernard, Hyeongwoo Kim, Patrick Pérez, Christian Theobalt*<br>


- **[Zhen-Hua Feng et al. (2018)](https://arxiv.org/abs/1803.05536)** (2018 FG) [[Code](https://github.com/patrikhuber/fg2018-competition)]<br>
**Evaluation of dense 3D reconstruction from 2D face images in the wild**<br>
*Zhen-Hua Feng, Patrik Huber, Josef Kittler, Peter JB Hancock, Xiao-Jun Wu, Qijun Zhao, Paul Koppen, Matthias Rätsch*<br>


- **[AffectNet](https://arxiv.org/abs/1708.03985)** (2017 TAC) [[Code](http://mohammadmahoor.com/affectnet/)]<br>
**AffectNet: A Database for Facial Expression, Valence, and Arousal Computing in the Wild**<br>
*Ali Mollahosseini, Behzad Hasani, Mohammad H. Mahoor*<br>


- **[3DMM-CNN](https://arxiv.org/pdf/1612.04904.pdf)** (2017 CVPR) [[Code](https://github.com/anhttran/3dmm_cnn)]<br>
**Regressing Robust and Discriminative 3D Morphable Models With a Very Deep Neural Network**<br>
*Anh Tuấn Trần, Tal Hassner, Iacopo Masi, Gerard Medioni*<br>


### 🫥 Facial/Head Models
<details>
  <summary>🪄 <b>Table of Contents</b></summary>

  - [3D Face Reconstruction](#3d-face-reconstruction)
    - 📑 [Papers](#-papers)
    - 🫥 [Facial/Head Models](#-facialhead-models)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks)
    - 📦 [Datasets](#-datasets)
  - [Face Animation with Audio (Talking Head)](#face-animation-with-audio-talking-head)
    - 📑 [Papers](#-papers-1)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks-1)
    - 📦 [Datasets](#-datasets-1)
</details>

- **[LYHM](https://link.springer.com/article/10.1007/s11263-019-01260-7)** (2020 ICCV) [[Link](https://www-users.york.ac.uk/~np7/research/LYHM/)]<br>
**Statistical Modeling of Craniofacial Shape and Texture**<br>
_Hang Dai, Nick Pears, William Smith, Christian Duncan_<br>
(*논문까지 읽을 필요는 없음*)

- **[FLAME](https://flame.is.tue.mpg.de/)** (2017 SIGGRAPH) ✨ [[Code](https://github.com/TimoBolkart/FLAME-Universe)]<br>
**Learning a model of facial shape and expression from 4D scans**<br>
*Tianye Li, Timo Bolkart, Michael J. Black, Hao Li, Javier Romero*<br>
3DMM 식 facial model. Shape, expression, pose 파라미터로 얼굴을 표현함. (*논문까지 읽을 필요는 없음*)


- **[BFM (Basel Face Model)](https://ieeexplore.ieee.org/document/5279762)** (2009 AVSS) ✨ [[Code](https://shapemodelling.cs.unibas.ch/web/)]<br>
**A 3D Face Model for Pose and Illumination Invariant Face Recognition**<br>
*Pascal Paysan, Reinhard Knothe, Brian Amberg, Sami Romdhani, Thomas Vetter*<br>
3DMM 식 facial model. FLAME 이전 및 FLAME과 함께 자주 사용되는 모델. (*논문까지 읽을 필요는 없음*)


- **[SCAPE](http://robots.stanford.edu/papers/anguelov.shapecomp.pdf)** (2005 SIGGRAPH) ✨<br>
**SCAPE: shape completion and animation of people**<br>
*Dragomir Anguelov, Praveen Srinivasan, Daphne Koller, Sebastian Thrun, Jim Rodgers, James Davis*<br>
 (*논문까지 읽을 필요는 없음*)


- **[3DMM](https://dl.acm.org/doi/10.1145/311535.311556)** (1999 SIGGRAPH) ✨<br>
**A morphable model for the synthesis of 3d faces**<br>
*Volker Blanz, Thomas Vetter*<br>
사람의 3D 모델링 방법으로, shape & texture를 vector space에서 표현하며, bases의 linear combination으로 표현 가능. *(논문까지 읽을 필요는 없음)*


### 🎖️ Leaderboards, Benchmarks
<details>
  <summary>🪄 <b>Table of Contents</b></summary>

  - [3D Face Reconstruction](#3d-face-reconstruction)
    - 📑 [Papers](#-papers)
    - 🫥 [Facial/Head Models](#-facialhead-models)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks)
    - 📦 [Datasets](#-datasets)
  - [Face Animation with Audio (Talking Head)](#face-animation-with-audio-talking-head)
    - 📑 [Papers](#-papers-1)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks-1)
    - 📦 [Datasets](#-datasets-1)
</details>

- **[NoW](https://now.is.tue.mpg.de/index.html)** (2019 CVPR) ✨<br>
사람 얼굴의 scan (GT)과 모델 결과의 mesh (prediction) 간의 거리를 측정해 median(↓), mean(↓), std(↓)를 비교. Expression, occlusion, varing views 상황을 구분하여 데이터셋을 구성함.


- **[REALY](https://realy3dface.com/)** (2022 ECCV)<br>


- **[Feng et al.(2018)]()** () ✨<br>
Scan (GT)과 recontructed mesh (prediction)를 rigid align 한 뒤, scan의 vertices로부터 가장 가까운 recontructed mesh (prediction) 상의 거리를 측정. (NoW와 유사)


- **[Stirling](https://pics.stir.ac.uk/ESRC/)** ()<br>



### 📦 Datasets

- **[MICA Dataset](https://zielon.github.io/mica/)** (2022 ECCV) [[Link](https://github.com/Zielon/MICA/tree/master/datasets)]<br>
**Towards Metrical Reconstruction of Human Faces**<br>
*Wojciech Zielonka, Timo Balkart, Justus Thies*<br>
MICA에서 여러 데이터셋을 모아 FLAME으로 fitting함.

- **[LYHM, Headspace Dataset](https://link.springer.com/article/10.1007/s11263-019-01260-7)** (2020 ICCV) [[Link](https://www-users.york.ac.uk/~np7/research/LYHM/)]<br>
**Statistical Modeling of Craniofacial Shape and Texture**<br>
_Hang Dai, Nick Pears, William Smith, Christian Duncan_<br>
LYHM head model 기반으로 만들어진 데이터셋.

* **[300W]()** () [[Link]()]<br>

* **[FRGC](https://cvrl.nd.edu/projects/data/#face-recognition-grand-challenge-frgc-v20-data-collection)** (2005 CVPR) [[Link]()]<br>
**Overview of the face recognition grand challenge**

- **[Stirling](https://pics.stir.ac.uk/ESRC/)** (2018 FG)<br>

- **[D3DFACS](https://www.cs.bath.ac.uk/~dpc/D3DFACS/ICCV_final_2011.pdf)** (2011 ICCV) [[Link](https://www.cs.bath.ac.uk/~dpc/D3DFACS/)]<br>
**A FACS Valid 3D Dynamic Action Unit Database with Applications to 3D Dynamic Morphable Facial Modeling**<br>
_Darren Cosker, Eva Krumhuber, Adrian Hilton_<br>

- **[Florence 2D/3D](https://dl.acm.org/doi/abs/10.1145/2072572.2072597)** (2011 J-HGBU) [[Link](https://www.micc.unifi.it/resources/datasets/florence-3d-faces/)]<br>
**The Florence 2D/3D Hybrid Face Dataset**<br>
_Andrew D. Bagdanov, Alberto Del Bimbo, Iacopo Masi_<br>

* **[FaceWarehouse](https://ieeexplore.ieee.org/document/6654137)** (2013 TVCG) [[Link](http://kunzhou.net/zjugaps/facewarehouse/)]<br>
**FaceWarehouse: A 3D Facial Expression Database for Visual Computing**<br>
*Chen Cao, Yanlin Weng, Shun Zhou, Yiying Tong, Kun Zhou*<br>

* **[AR database](https://portalrecerca.uab.cat/en/publications/the-ar-face-database-cvc-technical-report-24)** (1998) [[Link]()]<br>
**The ar face database**
_A.M. Martinez and R. Benavente_<br>


## Face Animation with Audio (Talking Head)
### 📑 Papers
<details>
  <summary>🪄 <b>Table of Contents</b></summary>

  - [3D Face Reconstruction](#3d-face-reconstruction)
    - 📑 [Papers](#-papers)
    - 🫥 [Facial/Head Models](#-facialhead-models)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks)
    - 📦 [Datasets](#-datasets)
  - [Face Animation with Audio (Talking Head)](#face-animation-with-audio-talking-head)
    - 📑 [Papers](#-papers-1)
    - 🎖️ [Leaderboards, Benchmarks](#%EF%B8%8F-leaderboards-benchmarks-1)
    - 📦 [Datasets](#-datasets-1)
</details>

- **[Speech4Mesh](https://openaccess.thecvf.com//content/ICCV2023/papers/He_Speech4Mesh_Speech-Assisted_Monocular_3D_Facial_Reconstruction_for_Speech-Driven_3D_Facial_ICCV_2023_paper.pdf)** (2023 ICCV)<br>
**Speech4Mesh: Speech-Assisted Monocular 3D Facial Reconstruction for Speech-Driven 3D Facial Animation**<br>
*Shan He, Haonan He, Shuo Yang, Xiaoyan Wu, Pengcheng Xia, Bing Yin, Cong Liu, LiRong Dai, Chang Xu*<br>


- **[EmoTalk](https://ziqiaopeng.github.io/emotalk/)** (2023 ICCV) [[Code](https://github.com/psyai-net/EmoTalk_release)]<br>
**EmoTalk: Speech-driven emotional disentanglement for 3D face animation**<br>
*Ziqiao Peng, Haoyu Wu, Zhenbo Song, Hao Xu, Xiangyu Zhu, Jun He, Hongyan Liu, Zhaoxin Fan*<br>


- **[SPECTRE](https://filby89.github.io/spectre/)** (2023 CVPR) ✨ [[Code](https://github.com/filby89/spectre)]<br>
**Visual Speech-Aware Perceptual 3D Facial Expression Reconstruction from Videos**<br>
*Panagiotis P. Filntisis, George Retsinas, Foivos Paraperas-Papantoniou, Athanasios Katsamanis, Anastasios Roussos, Petros Maragos*<br>


- **[CodeTalker](https://doubiiu.github.io/projects/codetalker/)** (2023 CVPR) [[Code](https://github.com/Doubiiu/CodeTalker)]<br>
**CodeTalker: Speech-Driven 3D Facial Animation with Discrete Motion Prior**<br>
*Jinbo Xing, Menghan Xia, Yuechen Zhang, Xiaodong Cun, Jue Wang, Tien-Tsin Wong*<br>


- **[SelfTalk](https://ziqiaopeng.github.io/selftalk/)** (2023 ACM MM) [[Code](https://github.com/psyai-net/SelfTalk_release)]<br>
**SelfTalk: A Self-Supervised Commutative Training Diagram to Comprehend 3D Talking Faces**<br>
*Ziqiao Peng, Yihao Luo, Yue Shi, Hao Xu, Xiangyu Zhu, Jun He, Hongyan Liu, Zhaoxin Fan*<br>
Lip shape을 더 정확하게 만들기 위해, 예측 결과 생성된 facial animation을 lip-reading interpreter에 넣어 text를 생성한 뒤, speech recognizer이 생성한 text와 비교함.


- **[MeshTalk](https://openaccess.thecvf.com/content/ICCV2021/html/Richard_MeshTalk_3D_Face_Animation_From_Speech_Using_Cross-Modality_Disentanglement_ICCV_2021_paper.html)** (2022 ICCV) [[Code](https://github.com/facebookresearch/meshtalk)]<br>
**MeshTalk: 3D Face Animation from Speech using Cross-Modality Disentanglement**<br>
*Alexander Richard, Michael Zollhofer, Yandong Wen, Fernando de la Torre, Yaser Sheikh*<br>
Latent space에서 audio-correlated와 uncorrelated information을 구분함. Lip shape와 upper face의 더 정확한 animation을 생성하고자 함.


- **[FaceFormer](https://evelynfan.github.io/audio2face/)** (2022 CVPR) ✨ [[Code](https://github.com/EvelynFan/FaceFormer)]<br>
**FaceFormer: Speech-Driven 3D Face Animation with Transformers**<br>
*Yingrou Fan, Zhaojiang Lin, Jun Saito, Wengping Wang, Taku Komura*<br>
Transformer-based 구조에 오디오를 context로 입력받아 autoregressive하게 face mesh를 생성.


- **[VOCA, VOCASET](https://voca.is.tue.mpg.de/)** (2019 CVPR) ✨ [[Code](https://github.com/TimoBolkart/voca)]<br>
**Capture, Learning, and Synthesis of 3D Speaking Styles**<br>
*Daniel Cudeiro, Timo Bolkart, Cassidy Laidlaw, Anurag Ranjan, Michael J. Black*<br>
Speaker-dependent였던 기존 연구와는 다르게, 오디오가 주어졌을 때 speaker-independent인 facial animation을 생성함. Speech가 있는 4D face scans로 이루어진 VOCASET 데이터셋 구축.


- **[Tero Karras et al. (2017)](https://research.nvidia.com/publication/2017-07_audio-driven-facial-animation-joint-end-end-learning-pose-and-emotion)** (2017 SIGGRAPH) ✨<br>
**Audio-driven facial animation by joint end-to-end learning of pose and emotion**<br>
*Tero Karras, Timo Aila, Samuli Laine, Antti Herva, Jaakko Lehtinen*<br>


- **[JALI](https://dl.acm.org/doi/abs/10.1145/2897824.2925984)** (2016 ToG)<br>
**JALI: an animator-centric viseme model for expressive lip synchronization**<br>
*Pif Edwards, Chris Landreth, Eugene Fiume, Karan Singh*<br>


### 📦 Datasets

* **[CelebV-HQ](https://celebv-hq.github.io/)** (2022 ECCV) ✨ [[Link](https://github.com/CelebV-HQ/CelebV-HQ/)]<br>
**CelebVHQ: A large-scale video facial attributes dataset**<br>
_Hao Zhu, Wayne Wu, Wentao Zhu, Liming Jiang, Siwei Tang, Li Zhang, Ziwei Liu, and Chen Change Loy_<br>
YouTube에서 수집된 비디오 데이터셋


* **[VoxCeleb2](https://arxiv.org/abs/1806.05622)** (2018 INTERSPEECH) ✨ [[Link](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox2.html)]<br>
**Voxceleb2: Deep speaker recognition**<br>
Joon Son Chung, Arsha Nagrani, Andrew Zisserman<br>
YouTube에서 수집된 비디오 데이터셋


- **[MEAD](https://wywu.github.io/projects/MEAD/support/MEAD.pdf)** (2019 ECCV) ✨ [[Link](https://github.com/uniBruce/Mead)]<br>
**Mead: A large-scale audio-visual dataset for emotional talking-face generation**<br>
_Kaisiyuan Wang, Qianyi Wu, Linsen Song, Zhuoqian Yang, Wayne Wu, Chen Qian, Ran He, Yu Qiao, Chen Change Loy_<br>
스튜디오에서 촬영된 비디오 데이터셋. Multi-view이며, emotion과 그 intensity를 다양하게 촬영함.


- **[VOCA, VOCASET](https://voca.is.tue.mpg.de/)** (2019 CVPR) ✨ [[Link](https://voca.is.tue.mpg.de/)]<br>
**Capture, Learning, and Synthesis of 3D Speaking Styles**<br>
*Daniel Cudeiro, Timo Bolkart, Cassidy Laidlaw, Anurag Ranjan, Michael J. Black*<br>
Speaker-dependent였던 기존 연구와는 다르게, 오디오가 주어졌을 때 speaker-independent인 facial animation을 생성함. Speech가 있는 4D face scans로 이루어진 VOCASET 데이터셋 구축.


* **[CoMA](https://coma.is.tue.mpg.de/)** (2018 ECCV)<br>
**Generating 3D faces using Convolutional Mesh Autoencoders**<br>
_Anurag Ranjan, Timo Bolkart, Soubhik Sanyal, Michael J. Black_<br>


* **[BIWI](https://ieeexplore.ieee.org/document/5571821)** (2010 TMM) [[Link](https://www.kaggle.com/datasets/kmader/biwi-kinect-head-pose-database/data)]<br>
**A 3-D Audio-Visual Corpus of Affective Communication**<br>
*Gabriele Fanelli, Thibaut Weise, Juergen Gall, Luc Van Gool*<br>
