<h1 align="center">Awesome 3D Face Reconstruction (Kor.)</h1>

<details>
<summary>Conference/Journal Name Abbr.</summary>

| Abbr. | Full name |
|-------|-----------|
|AVSS       |International Conference on Advanced Video and Signal Based Surveillance|
|CVPR       ||
|ICCV       ||
|ToG        ||
|SIGGRAPH   ||
|FG         |IEEE International Conference on Automatic Face & Gesture Recognition|
|TVCG       |IEEE Transactions on Visualization and Computer Graphics|
|TAG        |IEEE Transactions on Affective Computing|
</details>

## 3D Face Reconstruction
### Papers
> [!NOTE]
> arxiv 선공개 되었어도 이후 Conference 발표되었으면 그것을 기준으로 함.

**[AlbedoGAN](https://aashishrai3799.github.io/Towards-Realistic-Generative-3D-Face-Models/)** (2024 WACV) [[🖥️](https://github.com/aashishrai3799/Towards-Realistic-Generative-3D-Face-Models/)]<br>
**Towards Realistic Generative 3D Face Models**<br>
*Aashish Rai, Hiresh Gupta, Ayush Pandey, Francisco Vicente Carrasco, Shingo Jason Takagi, Amaury Aubel, Daeil Kim, Aayush Prakash, Fernando de la Torre*<br>
<ins> </ins>

**[TokenFace](https://openaccess.thecvf.com/content/ICCV2023/html/Zhang_Accurate_3D_Face_Reconstruction_with_Facial_Component_Tokens_ICCV_2023_paper.html)** (2023 ICCV)<br>
**Accurate 3D Face Reconstruction with Facial Component Tokens**<br>
*Tianke Zhang, Xuangeng Chu, Yunfei Liu, Lijian Lin, Zhendong Yang, Zhengzhuo Xu, Chengkun Cao, Fei Yu, Changyin Zhou, Chun Yuan, Yu Li*<br>
<ins>FLAME의 각 파라미터를 decoupling하고자, ViT에 이미지 토큰과 더불어 파라미터를 각각 token으로 만들어 입력함. 2&3D dataset을 동시에 사용함.</ins>

**[HiFace](https://project-hiface.github.io/)** (2023 ICCV)<br>
**HiFace: High-Fidelity 3D Face Reconstruction by Learning Static and Dynamic Details**<br>
*Zenghao Chai, Tianke Zhang, Tianyu He, Xu Tan, Tadas  Baltrušaitis, HsiangTao Wu, Runnan Li, Sheng Zhao, Chun Yuan, Jiang Bian*<br>
<ins>Detail을 static detail과 dynamic detail로 나눔. Synthetic dataset을 사용하여 학습.</ins>

**[FOCUS](https://arxiv.org/pdf/2106.09614.pdf)** (2023 CVPR) [[🖥️](https://github.com/unibas-gravis/Occlusion-Robust-MoFA)]<br>
**Robust Model-based Face Reconstruction through Weakly-Supervised Outlier Segmentation**<br>
*Chunlu Li, Andreas Morel-Forster, Thomas Vetter, Bernhard Egger, and Adam Kortylewski*<br>
<ins>Reconstruction과 outlier segmentation을 동시에 수행하여 outlier에도 robust한 결과를 얻고자 함.</ins>

**[HRN](https://younglbw.github.io/HRN-homepage/)** (2023 CVPR) [[🖥️](https://github.com/youngLBW/HRN)]<br>
**A Hierarchical Representation Network for Accurate and Detailed Face Reconstruction from In-The-Wild Images**<br>
*Biwen Lei, Jianqiang Ren, Mengyang Feng, Miaomiao Cui, Xuansong Xie*<br>
<ins> </ins>

**[DenseLandmarks](https://microsoft.github.io/DenseLandmarks/)** (2022 ECCV)<br>
**3D Face Reconstruction with Dense Landmarks**<br>
*Erroll Wood, Tadas Baltrušaitis, Charlie Hewitt, Matthew Johnson, Jingjing Shen, Nikola Milosavljevic, Daniel Wilde, Stephan Garbin, Chirag Raman, Jamie Shotton, Toby Sharp, Ivan Stojiljkovic, Thomas J. Cashman, Julien Valentin*<br>
<ins>700개 이상의 dense landmarks를 uncertainty와 함께 예측함. Synthetic dataset를 사용해 정확한 annotation을 얻을 수 있었음.</ins>

**[MICA](https://zielon.github.io/mica/)** (2022 ECCV) [[🖥️](https://github.com/Zielon/MICA)]<br>
**Towards Metrical Reconstruction of Human Faces**<br>
*Wojciech Zielonka, Timo Balkart, Justus Thies*<br>
<ins>Metrical한 reconstruction을 수행함. Pre-trained face reconstruction model에서 추출한 feature를 사용함으로써 서로 다른 얼굴에 대한 구분성을 높임. 여러 데이터셋을 합쳐 3D dataset을 구축해 supervised learning을 함.</ins>

**[EMOCA](https://emoca.is.tue.mpg.de/)** (2022 CVPR) ✨ [[🖥️](https://github.com/radekd91/emoca)]<br>
**EMOCA: Emotion Driven Monocular Face Capture and Animation**<br>
*Radek Danecek, Michael Black, Timo Bolkart*<br>
<ins>Expression encoder를 추가로 사용함과 동시에, 입력 이미지와 reconstruction 사이의 emotion 차이로 loss를 부여함으로써, emotion이 잘 보존된 결과를 얻음.</ins>

**[SynergyNet](https://arxiv.org/pdf/2110.09772.pdf)** (2021 3DV) ✨ [[🖥️](https://github.com/choyingw/SynergyNet)]<br>
**Synergy between 3DMM and 3D Landmarks for Accurate 3D Facial Geometry**<br>
*Cho-Ying Wu, Qiangeng Xu, Ulrich Neumann*<br>
<ins> </ins>

**[Dib et al.](https://arxiv.org/pdf/2103.15432.pdf)** (2021 ICCV) ✨<br>
**Towards high fidelity monocular face reconstruction with rich reflectance using self-supervised learning and ray tracing**<br>
*Abdallah Dib, Cedric Thebault, Junghyun Ahn, Philippe-Henri Gosselin, Christian Theobalt, Louis Chevallier*<br>
<ins> </ins>

**[Fast-GANFIT](https://arxiv.org/abs/2105.07474)** (2021 TPAMI) ✨ [[🖥️](https://github.com/barisgecer/GANFit)]<br>
**Fast-GANFIT: Generative Adversarial Network for High Fidelity 3D Face Reconstruction**<br>
*Baris Gecer, Stylianos Ploumpis, Irene Kotsia, Stefanos Zafeiriou*<br>
<ins> </ins>

**[DECA](https://arxiv.org/pdf/2012.04012.pdf)** (2021 SIGGRAPH) ✨ [[🖥️](https://github.com/YadiraF/DECA)]<br>
**Learning an Animatable Detailed 3D Face Model from In-the-Wild Images**<br>
*Yao Feng, Haiwen Feng, Michael J. Black, Timo Bolkart*<br>
<ins>Detail을 displacement map으로 예측해 coarse shape에 합쳐 reconstruction을 구성하며, 이로써 다른 이미지의 expression에서 얻은 displacement map으로 교체도 가능. 이후 수많은 모델의 기본 모델로 사용됨.</ins>

**[3DDFA-V2](https://arxiv.org/pdf/2009.09960.pdf)** (2020 ECCV) [[🖥️](https://github.com/cleardusk/3DDFA_V2)]<br>
**Towards Fast, Accurate and Stable 3D Dense Face Alignment**<br>
*Jianzhu Guo, Xiangyu Zhu, Yang Yang, Fan Yang, Zhen Lei, Stan Z. Li*<br>
<ins> </ins>

**[MGCNet](https://arxiv.org/pdf/2007.12494.pdf)** (2020 ECCV) ✨ [[🖥️](https://github.com/jiaxiangshang/MGCNet)]<br>
**Self-Supervised Monocular 3D Face Reconstruction by Occlusion-Aware Multi-view Geometry Consistency**<br>
*Jiaxiang Shang, Tianwei Shen, Shiwei Li, Lei Zhou, Mingmin Zhen, Tian Fang, Long Quan*<br>
<ins> </ins>

**[UMDFA](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123470681.pdf)** (2020 ECCV) ✨<br>
**“Look Ma, no landmarks!” – Unsupervised, model-based dense face alignment**<br>
*Tatsuro Koizumi, William A. P. Smith*<br>
<ins> </ins>

**[GANFIT](https://arxiv.org/pdf/1902.05978.pdf)** (2019 CVPR) ✨ [[🖥️](https://github.com/barisgecer/GANFit)]<br>
**GANFIT: Generative Adversarial Network Fitting for High Fidelity 3D Face Reconstruction**<br>
*Baris Gecer, Stylianos Ploumpis, Irene Kotsia, Stefanos Zafeiriou*<br>
<ins> </ins>

**[Luan Tran et al.](https://arxiv.org/abs/1904.04933)** (2019 CVPR) ✨ [[🖥️](https://github.com/tranluan/Nonlinear_Face_3DMM)]<br>
**Towards High-Fidelity Nonlinear 3D Face Morphable Model**<br>
*Luan Tran, Feng Liu, Xiaoming Liu*<br>
<ins> </ins>

**[RingNet, NoW](https://arxiv.org/pdf/1905.06817.pdf)** (2019 CVPR) ✨ [[🖥️](https://github.com/soubhiksanyal/RingNet)]<br>
**Learning to Regress 3D Face Shape and Expression from an Image without 3D Supervision**<br>
*Soubhik Sanyal, Timo Bolkart, Haiwen Feng and Michael J. Black*<br>
<ins> </ins>

**[Deep3DFaceRecon](https://arxiv.org/pdf/1903.08527.pdf)** (2019 CVPRw) ✨ [[🖥️](https://github.com/microsoft/Deep3DFaceReconstruction)]<br>
**Accurate 3D Face Reconstruction with Weakly-Supervised Learing: From Single Image to Image Set**<br>
*Yu Deng, Jiaolong Yang, Sicheng Xu, Dong Chen, Yunde Jia, Xin Tong*<br>
<ins> </ins>

**[PRNet](https://arxiv.org/pdf/1803.07835.pdf)** (2018 ECCV) ✨ [[🖥️](https://github.com/YadiraF/PRNet)]<br>
**Joint 3D Face Reconstruction and Dense Alignment with Position Map Regression Network**<br>
*Yao Feng, Fan Wu, Xiaohu Shao, Yanfeng Wang, and Xi Zhou*<br>
<ins> </ins>

**[Anh Tuấn Trần et al.](https://openaccess.thecvf.com/content_cvpr_2018/html/Tran_Extreme_3D_Face_CVPR_2018_paper.html)** (2018 CVPR) ✨ [[🖥️](https://github.com/anhttran/extreme_3d_faces)]<br>
**Extreme 3D Face Reconstruction: Seeing Through Occlusions**<br>
*Anh Tuấn Trần, Tal Hassner, Iacopo Masi, Eran Paz, Yuval Nirkin, Gérard Medioni*<br>
<ins> </ins>

**[Ayush Tewari et al.](https://vcai.mpi-inf.mpg.de/projects/FML/)** (2018 CVPR) ✨<br>
**Self-supervised multi-level face model learning for monocular reconstruction at over 250 Hz**<br>
*Ayush Tewari, Michael Zollhöfer, Pablo Garrido, Florian Bernard, Hyeongwoo Kim, Patrick Pérez, Christian Theobalt*<br>
<ins> </ins>

**[Zhen-Hua Feng et al. (2018)](https://arxiv.org/abs/1803.05536)** (2018 FG) ✨ [[🖥️](https://github.com/patrikhuber/fg2018-competition)]<br>
**Evaluation of dense 3D reconstruction from 2D face images in the wild**<br>
*Zhen-Hua Feng, Patrik Huber, Josef Kittler, Peter JB Hancock, Xiao-Jun Wu, Qijun Zhao, Paul Koppen, Matthias Rätsch*<br>
<ins> </ins>

**[AffectNet](https://arxiv.org/abs/1708.03985)** (2017 TAC) ✨ [[🖥️](http://mohammadmahoor.com/affectnet/)]<br>
**AffectNet: A Database for Facial Expression, Valence, and Arousal Computing in the Wild**<br>
*Ali Mollahosseini, Behzad Hasani, Mohammad H. Mahoor*<br>
<ins> </ins>

**[3DMM-CNN](https://arxiv.org/pdf/1612.04904.pdf)** (2017 CVPR) ✨ [[🖥️](https://github.com/anhttran/3dmm_cnn)]<br>
**Regressing Robust and Discriminative 3D Morphable Models With a Very Deep Neural Network**<br>
*Anh Tuấn Trần, Tal Hassner, Iacopo Masi, Gerard Medioni*<br>
<ins> </ins>

**[3DMM](https://dl.acm.org/doi/10.1145/311535.311556)** (1999 SIGGRAPH) ✨<br>
**A morphable model for the synthesis of 3d faces**<br>
*Volker Blanz, Thomas Vetter*<br>
<ins>사람의 3D 모델링 방법으로, shape & texture를 vector space에서 표현하며, bases의 linear combination으로 표현 가능.</ins>

### Facial/Head Model

**[FLAME](https://flame.is.tue.mpg.de/)** (2017 SIGGRAPH) ✨ [[🖥️](https://github.com/TimoBolkart/FLAME-Universe)]<br>
**Learning a model of facial shape and expression from 4D scans**<br>
*Tianye Li, Timo Bolkart, Michael J. Black, Hao Li, Javier Romero*<br>
<ins>3DMM 식 facial model. Shape, expression, pose 파라미터로 얼굴을 표현함. (*논문까지 읽을 필요는 없음*)</ins>

**[BFM (Basel Face Model)](https://ieeexplore.ieee.org/document/5279762)** (2009 AVSS) ✨ [[🖥️](https://shapemodelling.cs.unibas.ch/web/)]<br>
**A 3D Face Model for Pose and Illumination Invariant Face Recognition**<br>
*Pascal Paysan, Reinhard Knothe, Brian Amberg, Sami Romdhani, Thomas Vetter*<br>
<ins>3DMM 식 facial model. FLAME 이전 및 FLAME과 함께 자주 사용되는 모델. (*논문까지 읽을 필요는 없음*)</ins>

**[SCAPE](http://robots.stanford.edu/papers/anguelov.shapecomp.pdf)** (2005 SIGGRAPH) ✨<br>
**SCAPE: shape completion and animation of people**<br>
*Dragomir Anguelov, Praveen Srinivasan, Daphne Koller, Sebastian Thrun, Jim Rodgers, James Davis*<br>
<ins> </ins>

### Leaderboard, Benchmarks
- [NoW]()
- [REALY]()

## Talking Head (Face Animation) (Visual + Audio)

**[Speech4Mesh](https://openaccess.thecvf.com//content/ICCV2023/papers/He_Speech4Mesh_Speech-Assisted_Monocular_3D_Facial_Reconstruction_for_Speech-Driven_3D_Facial_ICCV_2023_paper.pdf)** (2023 ICCV)<br>
**Speech4Mesh: Speech-Assisted Monocular 3D Facial Reconstruction for Speech-Driven 3D Facial Animation**<br>
*Shan He, Haonan He, Shuo Yang, Xiaoyan Wu, Pengcheng Xia, Bing Yin, Cong Liu, LiRong Dai, Chang Xu*<br>
<ins> </ins>

**[EmoTalk](https://ziqiaopeng.github.io/emotalk/)** (2023 ICCV) [[🖥️](https://github.com/psyai-net/EmoTalk_release)]<br>
**EmoTalk: Speech-driven emotional disentanglement for 3D face animation**<br>
*Ziqiao Peng, Haoyu Wu, Zhenbo Song, Hao Xu, Xiangyu Zhu, Jun He, Hongyan Liu, Zhaoxin Fan*<br>
<ins> </ins>

**[SPECTRE](https://filby89.github.io/spectre/)** (2023 CVPR) [[🖥️](https://github.com/filby89/spectre)]<br>
**Visual Speech-Aware Perceptual 3D Facial Expression Reconstruction from Videos**<br>
*Panagiotis P. Filntisis, George Retsinas, Foivos Paraperas-Papantoniou, Athanasios Katsamanis, Anastasios Roussos, Petros Maragos*<br>
<ins> </ins>

**[CodeTalker](https://doubiiu.github.io/projects/codetalker/)** (2023 CVPR) ✨ [[🖥️](https://github.com/Doubiiu/CodeTalker)]<br>
**CodeTalker: Speech-Driven 3D Facial Animation with Discrete Motion Prior**<br>
*Jinbo Xing, Menghan Xia, Yuechen Zhang, Xiaodong Cun, Jue Wang, Tien-Tsin Wong*<br>
<ins> </ins>

**[SelfTalk](https://ziqiaopeng.github.io/selftalk/)** (2023 ACM MM) [[🖥️](https://github.com/psyai-net/SelfTalk_release)]<br>
**SelfTalk: A Self-Supervised Commutative Training Diagram to Comprehend 3D Talking Faces**<br>
*Ziqiao Peng, Yihao Luo, Yue Shi, Hao Xu, Xiangyu Zhu, Jun He, Hongyan Liu, Zhaoxin Fan*<br>
<ins>Lip shape을 더 정확하게 만들기 위해, 예측 결과 생성된 facial animation을 lip-reading interpreter에 넣어 text를 생성한 뒤, speech recognizer이 생성한 text와 비교함.</ins>

**[MeshTalk](https://openaccess.thecvf.com/content/ICCV2021/html/Richard_MeshTalk_3D_Face_Animation_From_Speech_Using_Cross-Modality_Disentanglement_ICCV_2021_paper.html)** (2022 ICCV) [[🖥️](https://github.com/facebookresearch/meshtalk)]<br>
**MeshTalk: 3D Face Animation from Speech using Cross-Modality Disentanglement**<br>
*Alexander Richard, Michael Zollhofer, Yandong Wen, Fernando de la Torre, Yaser Sheikh*<br>
<ins>Latent space에서 audio-correlated와 uncorrelated information을 구분함. Lip shape와 upper face의 더 정확한 animation을 생성하고자 함.</ins>

**[FaceFormer](https://evelynfan.github.io/audio2face/)** (2022 CVPR) [[🖥️](https://github.com/EvelynFan/FaceFormer)]<br>
**FaceFormer: Speech-Driven 3D Face Animation with Transformers**<br>
*Yingrou Fan, Zhaojiang Lin, Jun Saito, Wengping Wang, Taku Komura*<br>
<ins>Transformer-based 구조에 오디오를 context로 입력받아 autoregressive하게 face mesh를 생성.</ins>

**[VOCA, VOCASET](https://voca.is.tue.mpg.de/)** (2019 CVPR) ✨ [[🖥️](https://github.com/TimoBolkart/voca)]<br>
**Capture, Learning, and Synthesis of 3D Speaking Styles**<br>
*Daniel Cudeiro, Timo Bolkart, Cassidy Laidlaw, Anurag Ranjan, Michael J. Black*<br>
<ins>Speaker-dependent였던 기존 연구와는 다르게, 오디오가 주어졌을 때 speaker-independent인 facial animation을 생성함. Speech가 있는 4D face scans로 이루어진 VOCASET 데이터셋 구축.</ins>

**[Tero Karras et al. (2017)](https://research.nvidia.com/publication/2017-07_audio-driven-facial-animation-joint-end-end-learning-pose-and-emotion)** (2017 SIGGRAPH) ✨<br>
**Audio-driven facial animation by joint end-to-end learning of pose and emotion**<br>
*Tero Karras, Timo Aila, Samuli Laine, Antti Herva, Jaakko Lehtinen*<br>
<ins> </ins>
