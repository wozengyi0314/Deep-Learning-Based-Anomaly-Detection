# Anomaly Detection and Localization

Anomaly: Samples that significantly deviate from the majority of data instances.

Contributed by Chunyang Zhang.

## [Content](#content)

<table>
<tr><td colspan="2"><a href="#survey-papers">1. Survey</a></td></tr> 
<tr><td colspan="2"><a href="#methods">2. Methods</a></td></tr>
<tr>
    <td>&ensp;<a href="#cnn">2.1 CNN</a></td>
    <td>&ensp;<a href="#autoencoder">2.2 AutoenEoder</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#transformer">2.3 Transformer</a></td>
    <td>&ensp;<a href="#gan">2.4 GAN</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#representation-learning">2.5 Representation Learning</a></td>
    <td>&ensp;<a href="#reinforcement-learning">2.6 Reinforcement Learning</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#diffusion-model">2.7 Diffusion Model</a></td>
    <td>&ensp;<a href="#graph-network">2.8 Graph Network</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#lstm">2.9 LSTM</a></td>
    <td>&ensp;<a href="#"></a></td>
</tr>
<tr><td colspan="2"><a href="#methods">3. Mechanism</a></td></tr>
<tr>
    <td>&ensp;<a href="#dataset">3.1 Dataset</a></td>
    <td>&ensp;<a href="#student–teacher">3.2 Student–Teacher</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#meta-learning">3.3 Meta Learning</a></td>
    <td>&ensp;<a href="#outlier-exposure">3.4 Outlier Exposure</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#information-theory">3.5 Information Theory</a></td>
    <td>&ensp;<a href="#"></a></td>
</tr>
</table>


## [Survey Papers](#content)
1. **A survey of single-scene video anomaly detection.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/document/9271895)

   *Bharathkumar Ramachandra, Michael J. Jones, and Ranga Raju Vatsavai.*

1. **Deep learning for anomaly detection: A review.** ACM Computing Surveys, 2022. [paper](https://dl.acm.org/doi/10.1145/3439950)

   *Guansong Pang, Chunhua Shen, Longbing Cao, and Anton Van Den Hengel.*

1. **A unifying review of deep and shallow anomaly detection.** Proceedings of the IEEE, 2020. [paper](https://ieeexplore.ieee.org/document/9347460)

   *Ruff, Lukas and Kauffmann, Jacob R. and Vandermeulen, Robert A. and Montavon, Grégoire and Samek, Wojciech and Kloft, Marius and Dietterich, Thomas G., and Müller, and Klaus-Robert.*

1. **A review on outlier/anomaly detection in time series data.** ACM Computing Surveys, 2022. [paper](https://dl.acm.org/doi/10.1145/3444690)

   *Ane Blázquez-García, Angel Conde, Usue Mori, and Jose A. Lozano.* 

1. **A comprehensive survey on graph anomaly detection with deep learning.** TKDE, 2021. [paper](https://ieeexplore.ieee.org/document/9565320)

   *Ma, Xiaoxiao and Wu, Jia and Xue, Shan and Yang, Jian and Zhou, Chuan and Sheng, Quan Z. and Xiong, Hui, and Akoglu, Leman.* 

1. **Transformers in time series: A survey.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.07125)

   *Qingsong Wen, Tian Zhou, Chaoli Zhang, Weiqi Chen, Ziqing Ma, Junchi Yan, and Liang Sun.*

1. **Deep learning approaches for anomaly-based intrusion detection systems: A survey, taxonomy, and open issues.** KBS, 2020. [paper](https://www.sciencedirect.com/science/article/pii/S0950705119304897)

   *Arwa Aldweesh, Abdelouahid Derhab, and Ahmed Z.Emam.* 

1. **Deep learning-based anomaly detection in cyber-physical systems: Progress and oportunities.** ACM Computing Surveys, 2022. [paper](https://dl.acm.org/doi/10.1145/3453155)

   *Yuan Luo, Ya Xiao, Long Cheng, Guojun Peng, and Danfeng (Daphne) Yao.* 

1. **Deep learning for time series anomaly detection: A survey.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.05244)

   *Zahra Zamanzadeh Darban, Geoffrey I. Webb, Shirui Pan, Charu C. Aggarwal, and Mahsa Salehi.* 

1. **A survey of deep learning-based network anomaly detection.** Cluster Computing, 2019. [paper](https://link.springer.com/article/10.1007/s10586-017-1117-8)

   *Donghwoon Kwon, Hyunjoo Kim, Jinoh Kim, Sang C. Suh, Ikkyun Kim, and Kuinam J. Kim.* 

1. **Survey on anomaly detection using data mining techniques.** Procedia Computer Science, 2015. [paper](https://www.sciencedirect.com/science/article/pii/S1877050915023479)

   *Shikha Agrawal and Jitendra Agrawal.* 

1. **Graph based anomaly detection and description: A survey.** Data Mining and Knowledge Discovery, 2015. [paper](https://link.springer.com/article/10.1007/s10618-014-0365-y)

   *Leman Akoglu, Hanghang Tong, and Danai Koutra.* 

1. **Real-time big data processing for anomaly detection: A Survey.** International Journal of Information Management, 2019. [paper](https://www.sciencedirect.com/science/article/abs/pii/S0268401218301658)

   *Riyaz Ahamed Ariyaluran Habeeb, Fariza Nasaruddin, Abdullah Gani, Ibrahim AbakerTargio Hashem, Ejaz Ahmed, and Muhammad Imran.* 

1. **A survey of network anomaly detection techniques.** Journal of Network and Computer Applications, 2016. [paper](https://www.sciencedirect.com/science/article/abs/pii/S1084804515002891)

    *Mohiuddin Ahmed, Abdun Naser Mahmood, and Jiankun Hu.* 

    **Domain anomaly detection in machine perception: A system architecture and taxonomy.** TPAMI, 2014. [paper](https://ieeexplore.ieee.org/document/6636290)

    *Josef Kittler, William Christmas, Teófilo de Campos, David Windridge, Fei Yan, and  John Illingworth; Magda Osman.* 


## [Methods](#content) 
### [CNN](#content)
1. **Learning memory-guided normality for anomaly detection.** CVPR, 2020. [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Park_Learning_Memory-Guided_Normality_for_Anomaly_Detection_CVPR_2020_paper.pdf)

   *Hyunjong Park, Jongyoun No, and Bumsub Ham.* 

1. **CutPaste: Self-supervised learning for anomaly detection and localization.** CVPR, 2021. [paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Li_CutPaste_Self-Supervised_Learning_for_Anomaly_Detection_and_Localization_CVPR_2021_paper.pdf)

   *Chun-Liang Li, Kihyuk Sohn, Jinsung Yoon, and Tomas Pfister.* 

1. **Object-centric auto-encoders and dummy anomalies for abnormal event detection in video.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Ionescu_Object-Centric_Auto-Encoders_and_Dummy_Anomalies_for_Abnormal_Event_Detection_in_CVPR_2019_paper.pdf)

   *Radu Tudor Ionescu, Fahad Shahbaz Khan, Mariana-Iuliana Georgescu, and Ling Shao.* 

1. **Grad-CAM: Visual explanations from deep networks via gradient-based localization.** ICCV, 2017. [paper](https://ieeexplore.ieee.org/document/8237336)

   *Ramprasaath R. Selvaraju, Michael Cogswell, Abhishek Das, Ramakrishna Vedantam, Devi Parikh, and Dhruv Batra.* 

1. **A deep neural network for unsupervised anomaly detection and diagnosis in multivariate time series data.** AAAI, 2019. [paper](https://dl.acm.org/doi/10.1609/aaai.v33i01.33011409)

   *Chuxu Zhang, Dongjin Song, Yuncong Chen, Xinyang Feng, Cristian Lumezanu, Wei Cheng, Jingchao Ni, Bo Zong, Haifeng Chen, and Nitesh V. Chawla.* 

1. **Real-world anomaly detection in surveillance videos.** CVPR, 2018. [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Sultani_Real-World_Anomaly_Detection_CVPR_2018_paper.pdf)

   *Waqas Sultani, Chen Chen, and Mubarak Shah.* 

1. **FastAno: Fast anomaly detection via spatio-temporal patch transformation.** WACV, 2022. [paper](https://openaccess.thecvf.com/content/WACV2022/papers/Park_FastAno_Fast_Anomaly_Detection_via_Spatio-Temporal_Patch_Transformation_WACV_2022_paper.pdf)

   *Chaewon Park, MyeongAh Cho, Minhyeok Lee, and Sangyoun Lee.* 

1. **Object class aware video anomaly detection through image translation.** CRV, 2022. [paper](https://www.computer.org/csdl/proceedings-article/crv/2022/977400a090/1GeCy7y5kgU)

   *Mohammad Baradaran and Robert Bergevin.* 

1. **Anomaly detection in video sequence with appearance-motion correspondence.** ICCV, 2019. [paper](https://ieeexplore.ieee.org/document/9009067)

   *Trong-Nguyen Nguyen and Jean Meunier.* 

1. **Joint detection and recounting of abnormal events by learning deep generic knowledge.** ICCV, 2017. [paper](https://openaccess.thecvf.com/content_iccv_2017/html/Hinami_Joint_Detection_and_ICCV_2017_paper.html)

   *Ryota Hinami, Tao Mei, and Shin’ichi Satoh.* 

1. **Deep-cascade: Cascading 3D deep neural networks for fast anomaly detection and localization in crowded scenes.** TIP, 2017. [paper](https://ieeexplore.ieee.org/abstract/document/7858798)

   *Mohammad Sabokrou, Mohsen Fayyaz, Mahmood Fathy, and Reinhard Klette.* 

### [AutoEncoder](#content)
1. **Graph regularized autoencoder and its application in unsupervised anomaly detection.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/document/9380495)

   *Imtiaz Ahmed, Travis Galoppo, Xia Hu, and Yu Ding.* 

1. **Attention guided anomaly localization in images.** ECCV, 2020. [paper](https://link.springer.com/chapter/10.1007/978-3-030-58520-4_29)

   *Shashanka Venkataramanan, Kuan-Chuan Peng, Rajat Vikram Singh, and Abhijit Mahalanobis.* 

1. **A multimodal anomaly detector for robot-assisted feeding using an LSTM-based variational autoencoder.** ICRA, 2018. [paper](https://ieeexplore.ieee.org/abstract/document/8279425)

   *Daehyung Park, Yuuna Hoshi, and Charles C. Kemp.* 

1. **Anomaly detection using autoencoders in high performance computing systems.** AAAI, 2020. [paper](https://dl.acm.org/doi/10.1609/aaai.v33i01.33019428)

   *Andrea Borghesi, Andrea Bartolini, Michele Lombardi, Michela Milano, and Luca Benini.* 

1. **Deep autoencoding Gaussian mixture model for unsupervised anomaly detection.** ICLR, 2018. [paper](https://openreview.net/forum?id=BJJLHbb0-)

   *Bo Zongy, Qi Songz, Martin Renqiang Miny, Wei Chengy, Cristian Lumezanuy, Daeki Choy, and Haifeng Chen.* 

1. **Anomaly detection with robust deep autoencoders.** KDD, 2017. [paper](https://dl.acm.org/doi/10.1145/3097983.3098052)

   *Chong Zhou and Randy C. Paffenroth.* 

1. **Unsupervised anomaly detection via variational auto-encoder for seasonal KPIs in web applications.** WWW, 2018. [paper](https://dl.acm.org/doi/abs/10.1145/3178876.3185996)

   *Haowen Xu, Wenxiao Chen, Nengwen Zhao,Zeyan Li, Jiahao Bu, Zhihan Li, Ying Liu, Youjian Zhao, Dan Pei, Yang Feng, Jie Chen, Zhaogang Wang, and Honglin Qiao.* 

1. **Spatio-temporal autoencoder for video anomaly detection.** MM, 2017. [paper](https://dl.acm.org/doi/abs/10.1145/3123266.3123451)

   *Yiru Zhao, Bing Deng, Chen Shen, Yao Liu, Hongtao Lu, and Xiansheng Hua.* 

1. **Deep structured energy based models for anomaly detection.** ICML, 2016. [paper](https://dl.acm.org/doi/10.5555/3045390.3045507)

   *Shuangfei Zhai, Yu Cheng, Weining Lu, and Zhongfei Zhang.* 

1. **Learning discriminative reconstructions for unsupervised outlier removal.** ICCV, 2015. [paper](https://ieeexplore.ieee.org/document/7410534)

   *Yan Xia, Xudong Cao, Fang Wen, Gang Hua, and  Jian Sun.* 

1. **Outlier detection with autoencoder ensembles.** ICDM, 2017. [paper](https://research.ibm.com/publications/outlier-detection-with-autoencoder-ensembles)

   *Jinghui Chen, Saket Sathey, Charu Aggarwaly, and Deepak Turaga.*

1. **A study of deep convolutional auto-encoders for anomaly detection in videos.** Pattern Recognition Letters, 2018. [paper](https://www.sciencedirect.com/science/article/pii/S0167865517302489)

   *Manassés Ribeiro, AndréEugênio Lazzaretti, and Heitor Silvério Lopes.*

1. **Classification-reconstruction learning for open-set recognition.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Yoshihashi_Classification-Reconstruction_Learning_for_Open-Set_Recognition_CVPR_2019_paper.pdf)

   *Ryota Yoshihashi, Shaodi You, Wen Shao, Makoto Iida, Rei Kawakami, and Takeshi Naemura.*

1. **Learning temporal regularity in video sequences.** CVPR, 2016. [paper](https://openaccess.thecvf.com/content_cvpr_2016/html/Hasan_Learning_Temporal_Regularity_CVPR_2016_paper.html)

   *Mahmudul Hasan, Jonghyun Choi, Jan Neumann, Amit K. Roy-Chowdhury, and Larry S. Davis.*

1. **Clustering driven deep autoencoder for video anomaly detection.** ECCV, 2020. [paper](https://link.springer.com/chapter/10.1007/978-3-030-58555-6_20)

   *Yunpeng Chang, Zhigang Tu, Wei Xie, and Junsong Yuan .*

### [Transformer](#content)
1. **TranAD: deep transformer networks for anomaly detection in multivariate time series data.** Proceedings of the VLDB Endowment, 2022. [paper](https://dl.acm.org/doi/abs/10.14778/3514061.3514067)

   *Shreshth Tuli, Giuliano Casale, and Nicholas R. Jennings.* 

1. **Anomaly transformer: Time series anomaly detection with association discrepancy.** ICLR, 2022. [paper](https://openreview.net/pdf?id=LzQQ89U1qm)

   *Jiehui Xu, Haixu Wu, Jianmin Wang, and Mingsheng Long.* 

1. **Deep anomaly detection using geometric transformations.** NIPS, 2018. [paper](https://papers.nips.cc/paper/2018/hash/5e62d03aec0d17facfc5355dd90d441c-Abstract.html)

   *Izhak Golan and Ran El-Yaniv.* 

1. **Detecting anomalies within time series using local neural transformations.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.03944)

   *Tim Schneider, Chen Qiu, Marius Kloft, Decky Aspandi Latif, Steffen Staab, Stephan Mandt, and Maja Rudolph.* 

1. **Inpainting transformer for anomaly detection.** ICIAP, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-031-06430-2_33)

   *Jonathan Pirnay and Keng Chai.* 

1. **Self-supervised and interpretable anomaly detection using network transformers.** arXiv, 2022. [paper](https://arxiv.org/abs/2202.12997)

   *Daniel L. Marino, Chathurika S. Wickramasinghe, Craig Rieger, and Milos Manic.* 

1. **Anomaly detection in surveillance videos using transformer based attention model.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.01524)

   *Kapil Deshpande, Narinder Singh Punn, Sanjay Kumar Sonbhadra, and Sonali Agarwal.* 

1. **Multi-contextual predictions with vision transformer for video anomaly detection.** arXiv, 2022. [paper](https://arxiv.org/abs/2206.08568?context=cs)

   *Joo-Yeon Lee, Woo-Jeoung Nam, and Seong-Whan Lee.* 

1. **Transformer based models for unsupervised anomaly segmentation in brain MR images.** arXiv, 2022. [paper](https://arxiv.org/abs/2207.02059)

   *Ahmed Ghorbel, Ahmed Aldahdooh, Shadi Albarqouni, and Wassim Hamidouche.* 

1. **HaloAE: An HaloNet based local transformer auto-encoder for anomaly detection and localization.** arXiv, 2022. [paper](https://arxiv.org/abs/2208.03486)

   *E. Mathian, H. Liu, L. Fernandez-Cuesta, D. Samaras, M. Foll, and L. Chen.* 

1. **VT-ADL: A vision transformer network for image anomaly detection and localization.** ISIE, 2021. [paper](https://ieeexplore.ieee.org/abstract/document/9576231)

   *Pankaj Mishra, Riccardo Verk, Daniele Fornasier, Claudio Piciarelli, and Gian Luca Foresti.* 

1. **AnoViT: Unsupervised anomaly detection and localization with vision Transformer-based encoder-decoder.** IEEE Access, 2022. [paper](https://ieeexplore.ieee.org/abstract/document/9765986)

   *Yunseung Lee and Pilsung Kang.* 

### [GAN](#content)
1. **Stabilizing adversarially learned one-class novelty detection using pseudo anomalies.** TIP, 2022. [paper](https://ieeexplore.ieee.org/abstract/document/9887825)

   *Muhammad Zaigham Zaheer, Jin-Ha Lee, Arif Mahmood, Marcella Astri, and Seung-Ik Lee.* 

1. **GAN ensemble for anomaly detection.** AAAI, 2021. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/16530)

   *Han, Xu, Xiaohui Chen, and Li-Ping Liu.* 

1. **GAN-based anomaly detection in imbalance problems.** ECCV, 2020. [paper](https://link.springer.com/chapter/10.1007/978-3-030-65414-6_11)

   *Junbong Kim, Kwanghee Jeong, Hyomin Choi, and Kisung Seo.* 

1. **Unsupervised anomaly detection with generative adversarial networks to guide marker discovery.** IPMI, 2017. [paper](https://link.springer.com/chapter/10.1007/978-3-319-59050-9_12)

   *Thomas Schlegl, Philipp Seeböck, Sebastian M. Waldstein, Ursula Schmidt-Erfurth, and Georg Langs.* 

1. **Adversarially learned anomaly detection.** ICDM, 2018. [paper](https://ieeexplore.ieee.org/document/8594897)

   *Houssam Zenati, Manon Romain, Chuan-Sheng Foo, Bruno Lecouat, and Vijay Chandrasekhar.* 

1. **Convolutional transformer based dual discriminator generative adversarial networks for video anomaly detection.** MM, 2021. [paper](https://dl.acm.org/doi/abs/10.1145/3474085.3475693)

   *Xinyang Feng, Dongjin Song, Yuncong Chen, Zhengzhang Chen, Jingchao Ni, and Haifeng Chen.* 

1. **USAD: Unsupervised anomaly detection on multivariate time series.** KDD, 2020. [paper](https://dl.acm.org/doi/abs/10.1145/3394486.3403392)

   *Julien Audibert, Pietro Michiardi, Frédéric Guyard, Sébastien Marti, and Maria A. Zuluaga.* 

1. **Anomaly detection with generative adversarial networks for multivariate time series.** ICLR, 2018. [paper](https://arxiv.org/abs/1809.04758)

   *Dan Li, Dacheng Chen, Jonathan Goh, and See-kiong Ng.* 

1. **Efficient GAN-based anomaly detection.** ICLR, 2018. [paper](https://arxiv.org/abs/1802.06222)

   *Houssam Zenati, Chuan Sheng Foo, Bruno Lecouat, Gaurav Manek, and Vijay Ramaseshan Chandrasekhar.* 

1. **GANomaly: Semi-supervised Anomaly Detection via Adversarial Training.** ACCV, 2019. [paper](https://link.springer.com/chapter/10.1007/978-3-030-20893-6_39)

   *Akcay, Samet, Amir Atapour-Abarghouei, and Toby P. Breckon.* 

1. **f-AnoGAN: Fast unsupervised anomaly detection with generative adversarial networks.** Medical Image Analysis, 2019. [paper](https://www.sciencedirect.com/science/article/pii/S1361841518302640)

   *Thomas Schlegl , Philipp Seeböck, Sebastian M. Waldstein, Georg Langs, and Ursula Schmidt-Erfurth.* 

1. **OCGAN: One-class novelty detection using GANs with constrained latent
representations.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Perera_OCGAN_One-Class_Novelty_Detection_Using_GANs_With_Constrained_Latent_Representations_CVPR_2019_paper.pdf)

   *Pramuditha Perera, Ramesh Nallapati, and Bing Xiang.* 

1. **Adversarially learned one-class classifier for novelty detection.** CVPR, 2018. [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Sabokrou_Adversarially_Learned_One-Class_CVPR_2018_paper.pdf)

   *Mohammad Sabokrou, Mohammad Khalooei, Mahmood Fathy, and Ehsan Adeli.* 

1. **Generative probabilistic novelty detection with adversarial autoencoders.** NIPS, 2018. [paper](https://dl.acm.org/doi/10.5555/3327757.3327787)

   *Stanislav Pidhorskyi, Ranya Almohsen, Donald A. Adjeroh, and Gianfranco Doretto.* 

### [Flow](#content)
1. **OneFlow: One-class flow for anomaly detection based on a minimal volume region.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/abstract/document/9525256)

   *Lukasz Maziarka , Marek Smieja , Marcin Sendera , Lukasz Struski, Jacek Tabor, and Przemyslaw Spurek.* 
   
1. **Future frame prediction network for video anomaly detection.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/abstract/document/9622181/)

   *Weixin Luo, Wen Liu, Dongze Lian, and Shenghua Gao.* 
   
1. **Cloze test helps: Effective video anomaly detection via learning to complete video events.** MM, 2020. [paper](https://dl.acm.org/doi/abs/10.1145/3394171.3413973)

   *Guang Yu, Siqi Wang, Zhiping Cai, En Zhu, Chuanfu Xu, Jianping Yin, and Marius Kloft.* 

### [Weak Supervise](#content)
1. **Localizing anomalies from weakly-labeled videos.** TIP, 2021. [paper](https://ieeexplore.ieee.org/document/9408419)

   *Hui Lv, Chuanwei Zhou, Zhen Cui, Chunyan Xu, Yong Li, and Jian Yang.* 

1. **Out-of-distribution detection using an ensemble of self supervised leave-out classifiers.** ECCV, 2018. [paper](https://link.springer.com/chapter/10.1007/978-3-030-01237-3_34)

   *Apoorv Vyas, Nataraj Jammalamadaka, Xia Zhu, Dipankar Das, Bharat Kaul, and Theodore L. Willke.* 

1. **Self-supervised learning for generalizable out-of-distribution detection.** AAAI, 2020. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/5966)

   *Sina Mohseni, Mandar Pitale, JBS Yadawa, and Zhangyang ang.* 
### [Manifold Learning](#content)
1. **Real-time nonparametric anomaly detection in high-dimensional settings.** TPAMI, 2021. [paper](https://ieeexplore.ieee.org/abstract/document/8976215/)

   *Mehmet Necip Kurt, Yasin Yılmaz, and Xiaodong Wang.* 

### [Representation Learning](#content)
1. **AnomalyHop: An SSL-based image anomaly localization method.** International Conference on Visual Communications and Image Processing, 2021. [paper](https://ieeexplore.ieee.org/abstract/document/9675385)

   *Kaitai Zhang, Bin Wang, Wei Wang, Fahad Sohrab, Moncef Gabbouj, and C.-C. Jay Kuo.* 

1. **Learning representations of ultrahigh-dimensional data for random distance-based outlier detection.** KDD, 2018. [paper](https://dl.acm.org/doi/abs/10.1145/3219819.3220042)

   *Guansong Pang, Longbing Cao, Ling Chen, and Huan Liu.* 

1. **Federated disentangled representation learning for unsupervised brain anomaly detection.** Nature Machine Intelligence, 2022. [paper](https://www.nature.com/articles/s42256-022-00515-2)

   *Cosmin I. Bercea, Benedikt Wiestler, Daniel Rueckert, and Shadi Albarqouni.* 

1. **DSR–A dual subspace re-projection network for surface anomaly detection.** ECCV, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-031-19821-2_31)

   *Vitjan Zavrtanik, Matej Kristan, and Danijel Skočaj.* 

1. **Glancing at the patch: Anomaly localization with global and local feature comparison.** CVPR, 2021. [paper](https://openaccess.thecvf.com/content/CVPR2021/html/Wang_Glancing_at_the_Patch_Anomaly_Localization_With_Global_and_Local_CVPR_2021_paper.html)

   *Shenzhi Wang, Liwei Wu, Lei Cui, and Yujun Shen.* 

### [Sparse Representation](#content)
1. **Video anomaly detection with sparse coding inspired deep neural networks.** TPAMI, 2021. [paper](https://ieeexplore.ieee.org/abstract/document/8851288/)

   *Weixin Luo, Wen Liu, Dongze Lian, Jinhui Tang, Lixin Duan, Xi Peng, and Shenghua Gao.* 

1. **Self-supervised sparse representation for video anomaly detection.** ECCV, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-031-19778-9_42)

   *Jhihciang Wu, Heyen Hsieh, Dingjie Chen, Chioushann Fuh, and Tyngluh Liu.* 

1. **A revisit of sparse coding based anomaly detection in stacked RNN framework.** ICCV, 2017. [paper](https://link.springer.com/chapter/10.1007/978-3-031-19778-9_42)

   *Weixin Luo, Wen Liu, and Shenghua Gao.* 

### [Reinforcement Learning](#content)
1. **Towards experienced anomaly detector through reinforcement learning.** AAAI, 2018. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/12130)

   *Chengqiang Huang, Yulei Wu, Yuan Zuo, Ke Pei, and Geyong Min.* 

1. **Sequential anomaly detection using inverse reinforcement learning.** KDD, 2019. [paper](https://dl.acm.org/doi/10.1145/3292500.3330932)

   *Min-hwan Oh and Garud Iyengar.* 

1. **Toward deep supervised anomaly detection: Reinforcement learning from partially labeled anomaly data.** KDD, 2021. [paper](https://dl.acm.org/doi/10.1145/3447548.3467417)

   *Guansong Pang, Anton van den Hengel, Chunhua Shen, and Longbing Cao.* 

1. **Automated anomaly detection via curiosity-guided search and self-imitation learning.** TNNLS, 2021. [paper](https://ieeexplore.ieee.org/abstract/document/9526875)

   *Yuening Li, Zhengzhang Chen, Daochen Zha, Kaixiong Zhou, Haifeng Jin, Haifeng Chen, and Xia Hu.* 

1. **Meta-AAD: Active anomaly detection with deep reinforcement learning.** ICDM, 2020. [paper](https://ieeexplore.ieee.org/document/9338270)

   *Daochen Zha, Kwei-Herng Lai, Mingyang Wan, and Xia Hu.* 

### [Diffusion Model](#content)
1. **AnoDDPM: Anomaly detection with denoising diffusion probabilistic models using simplex noise.** CVPR, 2022. [paper](https://openaccess.thecvf.com/content/CVPR2022W/NTIRE/html/Wyatt_AnoDDPM_Anomaly_Detection_With_Denoising_Diffusion_Probabilistic_Models_Using_Simplex_CVPRW_2022_paper.html)

   *Julian Wyatt, Adam Leach, Sebastian M. Schmon, and Chris G. Willcocks.* 

1. **Diffusion models for medical anomaly detection.** MICCAI, 2022. [paper](https://link.springer.com/chapter/10.1007/978-3-031-16452-1_4)

   *Julia Wolleb, Florentin Bieder, Robin Sandkühler, and Philippe C. Cattin.* 

### [Graph Network](#content)
1. **Graph convolutional label noise cleaner: Train a plug-and-play action classifier for anomaly detection.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Zhong_Graph_Convolutional_Label_Noise_Cleaner_Train_a_Plug-And-Play_Action_Classifier_CVPR_2019_paper.html)

   *Jia-Xing Zhong, Nannan Li, Weijie Kong, Shan Liu, Thomas H. Li, and Ge Li.* 


1. **Decoupling representation learning and classification for GNN-based anomaly detection.** SIGIR, 2021. [paper](https://dl.acm.org/doi/10.1145/3404835.3462944)

   *Yanling Wan,, Jing Zhang, Shasha Guo, Hongzhi Yin, Cuiping Li, and Hong Chen.* 

1. **Rethinking graph neural networks for anomaly detection.** ICML, 2022. [paper](https://proceedings.mlr.press/v162/tang22b/tang22b.pdf)

   *Jianheng Tang,  Jiajin Li, Ziqi Gao, and Jia Li.* 

1. **NetWalk: A flexible deep embedding approach for anomaly detection in dynamic networks.** KDD, 2018. [paper](https://dl.acm.org/doi/10.1145/3219819.3220024)

   *Wenchao Yu, Wei Cheng, Charu C. Aggarwal, Kai Zhang, Haifeng Chen, and Wei Wang.* 

1. **LUNAR: Unifying local outlier detection methods via graph neural networks.** AAAI, 2022. [paper](https://ojs.aaai.org/index.php/AAAI/article/view/20629)

   *Adam Goodge, Bryan Hooi, See-Kiong Ng, and Wee Siong Ng.* 

### [Support Vector](#content)
1. **Patch SVDD: Patch-level SVDD for anomaly detection and segmentation.** ACCV, 2020. [paper](https://link.springer.com/chapter/10.1007/978-3-030-69544-6_23)

   *Jihun Yi and Sungroh Yoon.* 

### [LSTM](#content)
1. **Variational LSTM enhanced anomaly detection for industrial big data.** TII, 2021. [paper](https://ieeexplore.ieee.org/abstract/document/9195000)

   *Xiaokang Zhou, Yiyong Hu, Wei Liang, Jianhua Ma, and Qun Jin.* 
   
1. **Robust anomaly detection for multivariate time series through stochastic recurrent neuralnetwork.** KDD, 2019. [paper](https://dl.acm.org/doi/10.1145/3292500.3330672)

   *Ya Su, Youjian Zhao, Chenhao Niu, Rong Liu, Wei Sun, and Dan Pei.* 

1. **DeepLog: Anomaly detection and diagnosis from system logs through deep learning.** CCS, 2017. [paper](https://dl.acm.org/doi/10.1145/3133956.3134015)

   *Min Du, Feifei Li, Guineng Zheng, and Vivek Srikumar.* 

1. **Unsupervised anomaly detection with LSTM neural networks.** TNNLS, 2019. [paper](https://ieeexplore.ieee.org/abstract/document/8836638)

   *Tolga Ergen and Suleyman Serdar Kozat.* 
   
1. **LogAnomaly: Unsupervised detection of sequential and quantitative anomalies in unstructured logs.** IJCAI, 2019. [paper](https://www.ijcai.org/proceedings/2019/658)

   *Weibin Meng, Ying Liu, Yichen Zhu, Shenglin Zhang, Dan Pei, Yuqing Liu, Yihao Chen, Ruizhi Zhang, Shimin Tao, Pei Sun, and Rong Zhou.* 

1. **Outlier detection for time series with recurrent autoencoder ensembles.** IJCAI, 2019. [paper](https://dl.acm.org/doi/abs/10.5555/3367243.3367418)

   *Tung Kieu, Bin Yang, Chenjuan Guo, and Christian S. Jensen.* 

1. **Learning regularity in skeleton trajectories for anomaly detection in videos.** CVPR, 2019. [paper](https://dl.acm.org/doi/abs/10.5555/3367243.3367418)

   *Romero Morais, Vuong Le, Truyen Tran, Budhaditya Saha, Moussa Mansour, and Svetha Venkatesh.* 


## [Mechanism](#content)
### [Dataset](#content)
1. **DoTA: Unsupervised detection of traffic anomaly in driving videos.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/document/9712446)

   *Yu Yao, Xizi Wang, Mingze Xu, Zelin Pu, Yuchen Wang, Ella Atkins, and David Crandall.* 

1. **Street Scene: A new dataset and evaluation protocol for video anomaly detection.** WACV, 2020. [paper](https://openaccess.thecvf.com/content_WACV_2020/papers/Ramachandra_Street_Scene_A_new_dataset_and_evaluation_protocol_for_video_WACV_2020_paper.pdf)

   *Bharathkumar Ramachandra and Michael J. Jones.*

1. **Not only look, but also listen: Learning multimodal violence detection under weak supervision.** ECCV, 2020. [paper](https://link.springer.com/chapter/10.1007/978-3-030-58577-8_20)

   *Peng Wu, Jing Liu, Yujia Shi, Yujia Sun, Fangtao Shao, Zhaoyang Wu, and Zhiwei Yang.* 

1. **A revisit of sparse coding based anomaly detection in stacked RNN framework.** ICCV, 2017. [paper](https://openaccess.thecvf.com/content_iccv_2017/html/Luo_A_Revisit_of_ICCV_2017_paper.html)

   *Weixin Luo, Wen Liu, and Shenghua Gao.* 

1. **MVTec AD-A comprehensive real-world dataset for unsupervised anomaly detection.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Bergmann_MVTec_AD_--_A_Comprehensive_Real-World_Dataset_for_Unsupervised_Anomaly_CVPR_2019_paper.html)

   *Paul Bergmann, Michael Fauser, David Sattlegger, and Carsten Steger.* 

1. **Anomaly detection in crowded scenes.** CVPR, 2010. [paper](https://ieeexplore.ieee.org/abstract/document/5539872/)

   *Vijay Mahadevan, Weixin Li, Viral Bhalodia, and Nuno Vasconcelos.* 

1. **Abnormal event detection at 150 FPS in MATLAB.** ICCV, 2013. [paper](https://www.cv-foundation.org/openaccess/content_iccv_2013/html/Lu_Abnormal_Event_Detection_2013_ICCV_paper.html)

   *Cewu Lu, Jianping Shi, and Jiaya Jia.* 

1. **Surface defect saliency of magnetic tile.** The Visual Computer, 2020. [paper](https://link.springer.com/article/10.1007/s00371-018-1588-5)

   *Yibin Huang, Congying Qiu, and Kui Yuan .* 

### [library](#content)
1. **PyOD: A python toolbox for scalable outlier detection.** JMLR, 2019. [paper](https://www.jmlr.org/papers/v20/19-011.html)

   *Yue Zhao, Zain Nasrullah, and Zheng Li.* 

1. **OpenOOD: Benchmarking generalized out-of-distribution detection.** NIPS, 2022. [paper](https://arxiv.org/pdf/2210.07242.pdf)

   *Jingkang Yang, Pengyun Wang, Dejian Zou, Zitang Zhou, Kunyuan Ding, Wenxuan Peng, Haoqi Wang, Guangyao Chen, Bo Li, Yiyou Sun, Xuefeng Du,Kaiyang Zhou, Wayne Zhang, Dan Hendrycks, Yixuan Li, and Ziwei Liu.* 

### [Analysis](#content)
1. **Are we certain it’s anomalous?** arXiv, 2022. [paper](https://arxiv.org/pdf/2211.09224.pdf)

   *Alessandro Flaborea , Bardh Prenkaj , Bharti Munjal , Marco Aurelio Sterpa , Dario Aragona, Luca Podo, and Fabio Galasso.* 

1. **Learning causal temporal relation and feature discrimination for anomaly detection.** TIP, 2021. [paper](https://ieeexplore.ieee.org/document/9369126)

   *Peng Wu and Jing Liu.* 

1. **Anomaly detection requires better representations.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.10773)

   *Tal Reiss, Niv Cohen, Eliahu Horwitz, Ron Abutbul, and Yedid Hoshen.* 

1. **FAPM: Fast adaptive patch memory for real-time industrial anomaly detection.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.07548)

   *Shinji Yamada, Satoshi Kamiya, and Kazuhiro Hotta.* 

1. **Unsupervised model selection for time-series anomaly detection.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.01078)

   *Mononito Goswami, Cristian Challu, Laurent Callot, Lenon Minorics, and Andrey Kan.* 

1. **LGN-Net: Local-global normality network for video anomaly detection.** arXiv, 2022. [paper](https://arxiv.org/abs/2211.07454)

   *Mengyang Zhao, Yang Liu, Jing Liu, Di Li, and  Xinhua Zeng.* 

1. **Detecting data errors: Where are we and what needs to be done?** Proceedings of the VLDB Endowment, 2016. [paper](https://dl.acm.org/doi/10.14778/2994509.2994518)

   *Ziawasch Abedjan, Xu Chu, Dong Deng, Raul Castro Fernandez, Ihab F. Ilyas, Mourad Ouzzani, Paolo Papotti, Michael Stonebraker, and Nan Tang.* 

1. **Data cleaning: Overview and emerging challenges.** KDD, 2015. [paper](https://dl.acm.org/doi/10.1145/2882903.2912574)

   *Xu Chu, Ihab F. Ilyas, Sanjay Krishnan, and Jiannan Wang.* 

1. **Unmasking the abnormal events in video.** ICCV, 2017. [paper](https://dl.acm.org/doi/10.1145/2882903.2912574)

   *Radu Tudor Ionescu, Sorina Smeureanu, Bogdan Alexe, and Marius Popescu.* 
   
1. **Incorporating expert feedback into active anomaly discovery.** ICDM, 2016. [paper](https://ieeexplore.ieee.org/document/7837915)

   *Shubhomoy Das, Weng-Keen Wong, Thomas Dietterich, Alan Fern, and Andrew Emmott.* 
   
1. **Temporal cycle-consistency learning.** CVPR, 2019. [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Dwibedi_Temporal_Cycle-Consistency_Learning_CVPR_2019_paper.pdf)

   *Debidatta Dwibedi, Yusuf Aytar, Jonathan Tompson, Pierre Sermanet, and Andrew Zisserman.* 

### [Domain Adaptation](#content)
1. **Few-shot domain-adaptive anomaly detection for cross-site brain imagess.** TPAMI, 2022. [paper](https://ieeexplore.ieee.org/document/9606561)

   *Jianpo Su, Hui Shen, Limin Peng, and Dewen Hu.* 

### [Loss Function](#content)
1. **Detecting regions of maximal divergence for spatio-temporal anomaly detection.** TPAMI, 2018. [paper](https://ieeexplore.ieee.org/abstract/document/8352745)

   *Björn Barz, Erik Rodner, Yanira Guanche Garcia, and Joachim Denzler.* 

1. **Convex formulation for learning from positive and unlabeled data.** ICML, 2015. [paper](https://dl.acm.org/doi/10.5555/3045118.3045266)

   *Marthinus Christoffel Du Plessis, Gang Niu, and Masashi Sugiyama.* 

1. **Spatio-temporal autoencoder for  video anomaly detection.** MM, 2017. [paper](https://dl.acm.org/doi/abs/10.1145/3123266.3123451)

   *Yiru Zhao, Bing Deng, Chen Shen, Yao Liu, Hongtao Lu, and Xian-Sheng Hua.* 

### [Lifelong Learning](#content)
1. **Lifelong anomaly detection through unlearning.** CCS, 2019. [paper](https://dl.acm.org/doi/10.1145/3319535.3363226)

   *Min Du, Zhi Chen, Chang Liu, Rajvardhan Oak, and Dawn Song.* 

### [Student Teacher](#content)
1. **Uninformed students: Student-teacher anomaly detection with discriminative latent embeddings.** CVPR, 2020. [paper](https://openaccess.thecvf.com/content_CVPR_2020/html/Bergmann_Uninformed_Students_Student-Teacher_Anomaly_Detection_With_Discriminative_Latent_Embeddings_CVPR_2020_paper.html)

   *Paul Bergmann, Michael Fauser, David Sattlegger, and Carsten Steger.* 

1. **Reconstructed student-teacher and discriminative networks for anomaly detection.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.07548)

   *Shinji Yamada, Satoshi Kamiya, and Kazuhiro Hotta.* 

### [Data Augmentation](#content)
1. **Doping: Generative data augmentation for unsupervised anomaly detection with GAN.** ICDM, 2018. [paper](https://ieeexplore.ieee.org/abstract/document/8594955)

   *Swee Kiat Lim, Yi Loo, Ngoc-Trung Tran, Ngai-Man Cheung, Gemma Roig, and Yuval Elovici.* 

### [Memory Bank](#content)
1. **Towards total recall in industrial anomaly detection.** CVPR, 2022. [paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Roth_Towards_Total_Recall_in_Industrial_Anomaly_Detection_CVPR_2022_paper.pdf)

   *Karsten Roth, Latha Pemula, Joaquin Zepeda, Bernhard Schölkopf, Thomas Brox, and Peter Gehler.* 

1. **Memorizing normality to detect anomaly: Memory-augmented deep autoencoder for unsupervised anomaly detection.** ICCV, 2019. [paper](https://openaccess.thecvf.com/content_ICCV_2019/html/Gong_Memorizing_Normality_to_Detect_Anomaly_Memory-Augmented_Deep_Autoencoder_for_Unsupervised_ICCV_2019_paper.html)

   *Dong Gong, Lingqiao Liu, Vuong Le, Budhaditya Saha, Moussa Reda Mansour, Svetha Venkatesh, and Anton van den Hengel.* 

### [Gaussian Process](#content)
1. **Deep anomaly detection with deviation networks.** KDD, 2019. [paper](https://dl.acm.org/doi/10.1145/3292500.3330871)

   *Guansong Pang, Chunhua Shen, and Anton van den Hengel.* 

1. **Video anomaly detection and localization using hierarchical feature representation and Gaussian process regression.** CVPR, 2015. [paper](https://ieeexplore.ieee.org/document/7298909)

   *Kai-Wen Cheng and Yie-Tarng Chen, and Wen-Hsien Fang.* 

1. **Multidimensional time series anomaly detection: A GRU-based gaussian mixture variational autoencoder approach.** ACCV, 2018. [paper](http://proceedings.mlr.press/v95/guo18a.html)

   *Yifan Guo, Weixian Liao, Qianlong Wang, Lixing Yu, Tianxi Ji, and Pan Li.* 

1. **Gaussian process regression-based video anomaly detection and localization with hierarchical feature representation.** TIP, 2015. [paper](https://ieeexplore.ieee.org/abstract/document/7271067)

   *Kai-Wen Cheng, Yie-Tarng Chen, and Wen-Hsien Fang.* 

### [Meta Learning](#content)
1. **Learning unsupervised metaformer for anomaly detection.** CVPR, 2021. [paper](https://openaccess.thecvf.com/content/ICCV2021/html/Wu_Learning_Unsupervised_Metaformer_for_Anomaly_Detection_ICCV_2021_paper.html)

   *Jhih-Ciang Wu, Ding-Jie Chen, Chiou-Shann Fuh, and Tyng-Luh Liu.*

1. **Generic and scalable framework for automated time-series anomaly detection.** KDD, 2019. [paper](https://dl.acm.org/doi/10.1145/2783258.2788611)

   *Nikolay Laptev, Saeed Amizadeh, and Ian Flint.* 

### [Compact Feature](#content)
1. **Video anomaly detection with compact feature sets for online performance.** TIP, 2017. [paper](https://ieeexplore.ieee.org/abstract/document/7903693)

   *Roberto Leyva, Victor Sanchez, and Chang-Tsun Li.* 

### [Outlier Exposure](#content)
1. **Deep anomaly detection with outlier exposure.** ICLR, 2019. [paper](https://openreview.net/forum?id=HyxCxhRcY7)

   *Dan Hendrycks, Mantas Mazeika, and Thomas Dietterich.* 

### [Nearest Neighbor](#content)
1. **Online learning and sequential anomaly
   detection in trajectories.** TPAMI, 2014. [paper](https://ieeexplore.ieee.org/document/6598676)

   *Rikard Laxhammar and Göran Falkman.* 

### [Information Theory](#content)
1. **Deep semi-supervised anomaly detection.** ICLR, 2020. [paper](https://openreview.net/forum?id=HkgH0TEYwH)

   *Lukas Ruff, Robert A. Vandermeulen, Nico Görnitz, Alexander Binder, Emmanuel Müller, Klaus-Robert Müller, and Marius Kloft.* 

### [Density Estimation](#content)
1. **A discriminative framework for anomaly detection in large videos.** ECCV, 2016. [paper](https://link.springer.com/chapter/10.1007/978-3-319-46454-1_21)

   *Allison Del Giorno, J. Andrew Bagnell, and Martial Hebert.* 

1. **Hierarchical density estimates for data clustering, visualization, and outlier detection.** ACM Transactions on Knowledge Discovery from Data, 2015. [paper](https://dl.acm.org/doi/10.1145/2733381)

   *Ricardo J. G. B. Campello, Davoud Moulavi, Arthur Zimek, and Jörg Sander.* 


## [Application](#content)
### [Point Cloud](#content)
1. **Teacher-student network for 3D point cloud anomaly detection with few normal samples.** arXiv, 2022. [paper](https://arxiv.org/abs/2210.17258)

   *Jianjian Qin, Chunzhi Gu, Jun Yu, and Chao Zhang.* 

### [High Performance Computing](#content)
1. **Anomaly detection using autoencoders in high performance computing systems.** IAAI, 2019. [paper](https://dl.acm.org/doi/10.1609/aaai.v33i01.33019428)

   *Andrea Borghesi,  Andrea Bartolini, Michele Lombardi, Michela Milano, and Luca Benini.* 

### [Intrusion Detection](#content)
1. **Intrusion detection using convolutional neural networks for representation learning.** ICONIP, 2017. [paper](https://link.springer.com/chapter/10.1007/978-3-319-70139-4_87)

   *hipeng Li, Zheng Qin, Kai Huang, Xiao Yang, and Shuxiong Ye .* 

