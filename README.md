<!--
Copyright (c) 2022 lin

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
-->

<h3 align="center">
    <img src="https://github.com/linwhitehat/ETA-Resource/blob/main/ETA.png">
</h3>

<h1 align="center">
    <p>Encrypted Network Traffic Analysis Resources</p>
    <p>加密流量分析相关研究资源汇总</p>
</h1>

<p align="center">
    <a href="https://github.com/linwhitehat/ETA-Resource/blob/main/LICENSE">
        <img alt="GitHub" src="https://img.shields.io/github/license/linwhitehat/ETA-Resource.svg?color=green">
    </a>
    <img src="https://img.shields.io/github/stars/linwhitehat/ETA-Resource">
    <img src="https://img.shields.io/github/forks/linwhitehat/ETA-Resource">
    <a href="https://github.com/linwhitehat/ETA-Resource/graphs/traffic">
    <img src="https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Flinwhitehat%2FETA-Resource&label=visitor%20%20%20&labelColor=%23697689&countColor=%232ccce4&style=flat">
    </a>
    <a href="https://github.com/linwhitehat/ETA-Resource#contributors-"><img src="https://img.shields.io/badge/Contributors-6-orange.svg"></a>
</p>

**Note:**
- ⭐ **Please leave a <font color='orange'>STAR</font> if you like this project!** ⭐
- If you find any <font color='red'>incorrect</font> / <font color='red'>inappropriate</font> / <font color='red'>outdated</font> content, please kindly consider opening an issue or a PR. 
- We would greatly appreciate your contribution to this list, and you will appear in the [contributors✨](#contributors-)!

# Content
- [About](#about)
- [Dataset](#datasets)
- [Survey](#survey)
- [Network Traffic Analysis](#network-traffic-analysis)
- [Measurement](#measurement)
- [Teams](#teams)
- [Blogs](#blogs)
- [Libraries and Frameworks](#tool-libraries-and-frameworks)
<!--
- [Ethereum](#ethereum)
-->

# About
This is a current list of resources related to the research and development of encrypted traffic analysis. We comb the field for relevant representative work and related resources, and pay more attention to typical studies and research teams.

# Datasets
* [Canadian Institute for Cybersecurity Datasets](https://www.unb.ca/cic/datasets/) (DNS, IDS, DoS, Darknet, Tor, VPN, Botnet, Malware)
* [Information Security and Object Technology Research Lab Datasets](https://onlineacademiccommunity.uvic.ca/isot/datasets/) (IoT, Botnet, Cloud Security)
* [Cross-Platform](https://recon.meddle.mobi/cross-market.html) (iOS and Android Apps)
* [Malware Capture Facility Project](https://www.stratosphereips.org/datasets-overview) (Malware)
* [CSTNET-TLS 1.3](https://drive.google.com/drive/folders/1JSsYmevkxQFanoKOi_i1ooA6pH3s9sDr?usp=sharing) (TLS 1.3 services)
* [Network-based Intrusion Detection](https://www.sciencedirect.com/science/article/pii/S016740481930118X) (AWID, Botnet, CIC DoS, CICIDS, CIDDS, CTU, DARPA, ISCX, IRSC)
* [MobileTraffic](https://github.com/Abby-ZS/NUDT_MobileTraffic) (300+ Mobile Apps)
* [Itc-Net-Blend-60](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4661706) (Android applications in Diverse Environments)
* [Network-Flow-of-QUIC](https://drive.google.com/drive/folders/1cwHhzvaQbi-ap8yfrj2vHyPmUTQhaYOj) (QUIC services)
* [Network Multiflow Fingerprinting Datasets](https://www.kaggle.com/datasets/fuukaa/network-multiflow-fingerprinting-datasets?datasetId=3270419&select=Keyword+Search+Dataset+Pcap) (User Activities (UAV), IoT Device Identification (IDI), Intrusion Detection (ISD), Keyword Searching (KWS), Shadowsocks Website 
Fingerprinting (SWF))
* [CTU-13](https://mcfp.weebly.com/the-ctu-13-dataset-a-labeled-dataset-with-botnet-normal-and-background-traffic.html) (Botnet, Malware)
* [ANT Datasets](https://ant.isi.edu/datasets/index.html) (Botnet, IoT, DNS, IP Geolocation)
* [LFETT2021 Dataset](https://github.com/HoneyPotter-Gzy/LFETT2021-dataset) (Tunnel, Proxy, VPN)
* [AnonProxy2023](https://github.com/MrRobotsAA/AnonProxy2023-Dataset) (Anonymous, Proxy, VPN)
* [DataCon2021-加密代理流量数据集](https://datacon.qianxin.com/opendata/openpage?resourcesId=10) (Proxy, VPN)

# Survey
* [Machine Learning-Powered Encrypted Network Traffic Analysis: A Comprehensive Survey](https://ieeexplore.ieee.org/document/9896143). Meng Shen. IEEE Communications Surveys & Tutorials 2023.
* [Deep Learning for Encrypted Traffic Classification: An Overview](https://ieeexplore.ieee.org/document/8713803/). Shahbaz Rezaei. IEEE Communications Magazine 2019.
* [Towards the Deployment of Machine Learning Solutions in Network Traffic Classification: A Systematic Survey](https://ieeexplore.ieee.org/document/8543584). Fannia Pacheco. IEEE Communications Surveys & Tutorials 2019.
* [Deep Learning in Mobile and Wireless Networking: A Survey](https://ieeexplore.ieee.org/document/8666641). Chaoyun Zhang. IEEE Communications Surveys & Tutorials 2019.

# Network Traffic Analysis

## ETA with Pre-training/LLMs (Generalization, Side-channel Analysis)
* [TrafficFormer: An Efficient Pre-trained Model for Traffic Data](http://www.thucsnet.com/wp-content/papers/guangmeng_sp2025.pdf). Guangmeng Zhou. S&P 2025. [[code]](https://github.com/IDP-code/TrafficFormer)
* [What Was Your Prompt? A Remote Keylogging Attack on AI Assistants](https://www.usenix.org/conference/usenixsecurity24/presentation/weiss). Roy Weiss. USENIX 2024. [[code]](https://github.com/royweiss1/GPT_Keylogger)
* [CETP: A Novel Semi-Supervised Framework Based on Contrastive Pre-Training for Imbalanced Encrypted Traffic Classification](https://www.sciencedirect.com/science/article/abs/pii/S0167404824001949). Xinjie Lin. Computers & Security (ComSec) 2024.
* [A novel approach for application classification with encrypted traffic using BERT and packet headers](https://www.sciencedirect.com/science/article/pii/S1389128624005796). Jaehak Yu. Computer Networks 2024.
* [Flow-MAE: Leveraging Masked AutoEncoder for Accurate, Efficient and Robust Malicious Traffic Classification](https://dl.acm.org/doi/10.1145/3607199.3607206#core-collateral-purchase-access). Zijun Hang. RAID 2023. [[code]](https://github.com/NLear/Flow-MAE)
* [Listen to Minority: Encrypted Traffic Classification for Class Imbalance with Contrastive Pre-Training](https://ieeexplore.ieee.org/abstract/document/10287449). Xiang Li. SECON 2023.
* [Yet Another Traffic Classifier: A Masked Autoencoder Based Traffic Transformer with Multi-Level Flow Representation](https://ojs.aaai.org/index.php/AAAI/article/view/25674). Ruijie Zhao. AAAI 2023. [[code]](https://github.com/NSSL-SJTU/YaTC)
* [ET-BERT: A Contextualized Datagram Representation with Pre-training Transformers for Encrypted Traffic Classification](https://dl.acm.org/doi/abs/10.1145/3485447.3512217). Xinjie Lin. WWW 2022. [[code]](https://github.com/linwhitehat/et-bert) [[Reproduce]](https://gitee.com/xxdxxdxxd/et-bert/blob/master/README.md)

## ETA for Stable/Robust (Out-of-Distribution, Few-shot, Zero-shot)
* [CD-Net: Robust mobile traffic classification against apps updating](https://www.sciencedirect.com/science/article/abs/pii/S0167404824005200). Yanan Chen. ComSec 2025.
* [Robust and Reliable Early-Stage Website Fingerprinting Attacks via Spatial-Temporal Distribution Analysis](https://arxiv.org/pdf/2407.00918). Xinhao Deng. CCS 2024. [[code]](https://github.com/Xinhao-Deng/Website-Fingerprinting-Library)
* [Low-Quality Training Data Only? A Robust Framework for Detecting Encrypted Malicious Network Traffic](https://www.ndss-symposium.org/ndss-paper/low-quality-training-data-only-a-robust-framework-for-detecting-encrypted-malicious-network-traffic/). Yuqi Qing. NDSS 2024. [[code]](https://github.com/XXnormal/RAPIER)
* [Identifying malicious traffic under concept drift based on intraclass consistency enhanced variational autoencoder](http://scis.scichina.com/en/2024/182302.pdf). Xiang Luo. SCIENCE CHINA Information Sciences (SCIS) 2024.
* [TrafCL: Robust Encrypted Malicious Traffic Detection via Contrastive Learning](https://dl.acm.org/doi/abs/10.1145/3627673.3679839). Xiaodu Yang. CIKM 2024.
* [MCRe: A Unified Framework for Handling Malicious Traffic With Noise Labels Based on Multidimensional Constraint Representation](https://dl.acm.org/doi/10.1109/TIFS.2023.3318962). Qingjun Yuan. TIFS 2024.
* [Few-shot encrypted traffic classification via multi-task representation enhanced meta-learning](https://www.sciencedirect.com/science/article/pii/S1389128623001767). Chen Yang. Computer Networks 2023.
* [Rosetta: Enabling Robust TLS Encrypted Traffic Classification in Diverse Network Environments with TCP-Aware Traffic Augmentation](https://www.usenix.org/conference/usenixsecurity23/presentation/xie). Renjie Xie. USENIX 2023. [[code]](https://github.com/sunskyXX/Rosetta)
* [Zero-relabelling mobile-app identification over drifted encrypted network traffic](https://doi.org/10.1016/j.comnet.2023.109728). Minghao Jiang. Computer Networks 2023.
* [Anomaly Detection in the Open World: Normality Shift Detection, Explanation, and Adaptation](https://www.ndss-symposium.org/ndss-paper/anomaly-detection-in-the-open-world-normality-shift-detection-explanation-and-adaptation/). Dongqi Han. NDSS 2023. [[code]](https://github.com/dongtsi/OWAD)
* [Accurate mobile-app fingerprinting using flow-level relationship with graph neural networks](https://www.sciencedirect.com/science/article/pii/S1389128622003577). Minghao Jiang. Computer Networks 2022.
* [Triplet Fingerprinting: More Practical and Portable Website Fingerprinting with N-shot Learning](https://dl.acm.org/doi/abs/10.1145/3319535.3354217). Payap Sirinam. CCS 2019. [[code]](https://github.com/triplet-fingerprinting/tf) (N-shot Learning)

## Traditional Targets (Web, App, Malware, Gambling, User Activities, Intrusion Detection, IoT, Streaming Media)
* General
    * [FlowMiner: A Powerful Model Based on Flow Correlation Miningfor Encrypted Traffic Classification](). Hongbo Xu. INFOCOM 2025.
    * [DE-GNN: Dual embedding with graph neural network for fine-grained encrypted traffic classification](https://www.sciencedirect.com/science/article/pii/S1389128624002044). Xinbo Han. Computer Networks 2024.
    * [Towards Fine-Grained Webpage Fingerprinting at Scale](https://www.arxiv.org/abs/2409.04341). Xiyuan Zhao. CCS 2023.
    * [TFE-GNN: A Temporal Fusion Encoder Using Graph Neural Networks for Fine-grained Encrypted Trafic Classification](https://dl.acm.org/doi/abs/10.1145/3543507.3583227). Haozhen Zhang. WWW 2023. [[code]](https://github.com/ViktorAxelsen/TFE-GNN)
    * [An Input-Agnostic Hierarchical Deep Learning Framework for Traffic Fingerprinting](https://www.usenix.org/conference/usenixsecurity23/presentation/qu). Jian Qu. USENIX 2023. [[code]](https://github.com/shashadehuajiang/trace_classifier/tree/main)
    * [Classifying encrypted traffic using adaptive fingerprints with multi-level attributes](https://link.springer.com/article/10.1007%2Fs11280-021-00940-0). Chang Liu. WWW Journal 2021.
    * [CETAnalytics: Comprehensive effective traffic information analytics for encrypted traffic classification](https://www.sciencedirect.com/science/article/pii/S1389128619309466) (Generalization). Cong Dong. Computer Networks 2020.
    * [FlowPrint: Semi-Supervised Mobile-App Fingerprinting on Encrypted Network Traffic](https://www.ndss-symposium.org/wp-content/uploads/2020/02/24412.pdf). van Ede, Thijs. NDSS 2020. [[code]](https://github.com/Thijsvanede/FlowPrint)
    * [FS-Net: A Flow Sequence Network For Encrypted Traffic Classification](https://ieeexplore.ieee.org/document/8737507). Chang Liu. INFOCOM 2019. [[code]](https://github.com/WSPTTH/FS-Net)
    * [MaMPF: Encrypted Traffic Classification Based on Multi-Attribute Markov Probability Fingerprints](https://ieeexplore.ieee.org/abstract/document/8624124).  Chang Liu. IWQoS 2018. [[code]](https://github.com/WSPTTH/MaMPF)
    * [AppScanner: Automatic Fingerprinting of Smartphone Apps from Encrypted Network Traffic](https://ieeexplore.ieee.org/abstract/document/7467370). Vincent F. Taylor. EuroS&P 2016. [[code]](https://github.com/vftaylor/appscanner)
    * [Adaptive encrypted traffic fingerprinting with bi-directional dependence](https://dl.acm.org/doi/abs/10.1145/2991079.2991123). Khaled Al-Naami. ACSAC 2016. [[code]](https://github.com/khaled-alnaami/NetworkTrafficFingerprinting)
* Malicious
    * [PETNet: Plaintext-aware encrypted traffic detection network for identifying Cobalt Strike HTTPS traffics](https://www.sciencedirect.com/science/article/pii/S1389128623005650). Xiaodu Yang. Computer Networks 2024. [[code]](https://github.com/CN-PETNet/PETNet)
    * [Early Network Intrusion Detection Enabled by Attention Mechanisms and RNNs](https://doi.org/10.1109/TIFS.2024.3441862). Taki Eddine Toufik Djaidja. TIFS 2024.
    * [TMG-GAN: Generative Adversarial Networks-Based Imbalanced Learning for Network Intrusion Detection](https://dl.acm.org/doi/10.1109/TIFS.2023.3331240). Hongwei Ding. TIFS 2024.
    * [Point Cloud Analysis for ML-Based Malicious Traffic Detection: Reducing Majorities of False Positive Alarms](https://dl.acm.org/doi/10.1145/3576915.3616631). Chuanpu Fu. CCS 2023.
    * [Detecting Unknown Encrypted Malicious Traffic in Real Time via Flow Interaction Graph Analysis](https://www.ndss-symposium.org/wp-content/uploads/2023/02/ndss2023_s80_paper.pdf). Chuanpu Fu. NDSS 2023.
* Gambling
    * [Let gambling hide nowhere: Detecting illegal mobile gambling apps via heterogeneous graph-based encrypted traffic analysis](https://www.sciencedirect.com/science/article/pii/S1389128624001105). Zheyuan Gu. Computer Networks 2024.
    * [Gambling Domain Name Recognition via Certificate and Textual Analysis](https://academic.oup.com/comjnl/article/66/8/1829/6570684). GuoYing Sun. The Computer Journal 2023.
    * [Analyzing Ground-Truth Data of Mobile Gambling Scams](https://ieeexplore.ieee.org/abstract/document/9833665). Geng Hong. Symposium on Security and Privacy (S&P) 2022.
* IoT
    * [HorusEye: A Realtime IoT Malicious Traffic Detection Framework using Programmable Switches](https://www.usenix.org/conference/usenixsecurity23/presentation/dong-yutao). Yutao Dong. USENIX 2023.
* Vedio (Streaming Media)
    * [Breaking Through the Diversity: Encrypted Video Identification Attack Based on QUIC Features](https://link.springer.com/chapter/10.1007/978-3-031-70903-6_9#author-information). Nan Hu. ESORICS 2024.
    * [Traffic spills the beans: A robust video identification attack against YouTube](https://www.sciencedirect.com/science/article/abs/pii/S0167404823005333). Xiyuan Zhang. ComSec 2024.
    * [Walls Have Ears: Traffic-based Side-channel Attack in Video Streaming](https://ieeexplore.ieee.org/abstract/document/8486211). Jiaxi Gu. IEEE INFOCOM 2018.

## Defense and Adversarial Techniques
* [Real-Time Website Fingerprinting Defense via Traffic Cluster Anonymization](https://www.computer.org/csdl/proceedings-article/sp/2024/313000a263/1WPcZnZILHa). Meng Shen. S&P 2024.
* [Defending Against Deep Learning-Based Traffic Fingerprinting Attacks With Adversarial Examples](https://dl.acm.org/doi/abs/10.1145/3698591). Blake Hayden. ACM Transactions on Privacy and Security (TOPS) 2024.
* [Subverting Website Fingerprinting Defenses with Robust Traffic Representation](https://www.usenix.org/conference/usenixsecurity23/presentation/shen-meng). Meng Shen. USENIX 2023.

## Anonymous and VPN
* [Rules Refine the Riddle: Global Explanation for Deep Learning-Based Anomaly Detection in Security Applications](). DongqiHan. CCS 2024. [[code]](https://github.com/dongtsi/GEAD)
* [Detecting Tunneled Flooding Traffic via Deep Semantic Analysis of Packet Length Patterns](https://drive.google.com/file/d/1_P8HIs3Q9f_HlA9_x2HMr0q6ScPzrF0g/view). Chuanpu Fu. CCS 2024. [[code]](https://github.com/fuchuanpu/Exosphere) [[video]](https://www.bilibili.com/video/BV1QLCUYuEKM/?spm_id_from=333.1387.collection.video_card.click&vd_source=a1efd78c138281beaaf12f4f11412057)
* [ProxyKiller: An Anonymous Proxy Traffic Attack Model Based on Traffic Behavior Graphs](https://link.springer.com/chapter/10.1007/978-3-031-70890-9_9#Tab4). Hongbo Xu. ESORICS 2024.
* [HSDirSniper: A New Attack Exploiting Vulnerabilities in Tor's Hidden Service Directories](https://dl.acm.org/doi/10.1145/3589334.3645591). Qingfeng Zhang. WWW 2024.
* [VPNSniffer: Identifying VPN Servers Through Graph-Represented Behaviors](https://dl.acm.org/doi/10.1145/3589334.3645552). Chenxu Wang. WWW 2024.
* [AppSniffer: Towards Robust Mobile App Fingerprinting Against VPN](https://dl.acm.org/doi/10.1145/3543507.3583473). Sanghak Oh. WWW 2023.
* [Transformer-based Model for Multi-tab Website Fingerprinting Attack](https://dl.acm.org/doi/abs/10.1145/3576915.3623107). Zhaoxin Jin. CCS 2023.
* [Online Website Fingerprinting: Evaluating Website Fingerprinting Attacks on Tor in the Real World](https://www.usenix.org/conference/usenixsecurity22/presentation/cherubin). Giovanni Cherubin. USENIX 2022.
* [BAPM: Block Attention Profiling Model for Multi-tab Website Fingerprinting Attacks on Tor](https://dl.acm.org/doi/10.1145/3485832.3485891). Zhong Guan. ACSAC 2021.
* [Deep Fingerprinting: Undermining Website Fingerprinting Defenses with Deep Learning](https://dl.acm.org/doi/abs/10.1145/3243734.3243768). Payap Sirinam. CCS 2018. [[code]](https://github.com/deep-fingerprinting/df)

# Measurement
* Domain Name System
    * [A Worldwide View on the Reachability of Encrypted DNS Services](https://dl.acm.org/doi/abs/10.1145/3589334.3645539). Ruixuan Li. WWW 2024.
    * [Investigating Deployment Issues of DNS Root Server Instances from a China-wide View](https://ieeexplore.ieee.org/abstract/document/10460172/keywords#keywords). Fenglu Zhang. IEEE Transactions on Dependable and Secure Computing (TDSC) 2024.
* Privacy and Security
    * [Privacy protection of China’s top websites: A Multi-layer privacy measurement via network behaviours and privacy policies](https://www.sciencedirect.com/science/article/abs/pii/S0167404822000050). Xinjie Lin. ComSec 2022.
* IPv6
    * [IPv6 Prefix Target Generation through Pattern and Distribution Learning using Vision-Transformer and Guided-Diffusion](). Yaochen Ren. INFOCOM 2025.
    * [6GAN: IPv6 Multi-Pattern Target Generation via Generative Adversarial Nets with Reinforcement Learning](https://ieeexplore.ieee.org/document/9488912). Tianyu Cui. INFOCOM 2021. [[code]](https://github.com/CuiTianyu961030/6GAN)
    * [SiamHAN: IPv6 Address Correlation Attacks on TLS Encrypted Traffic via Siamese Heterogeneous Graph Attention Network](https://www.usenix.org/conference/usenixsecurity21/presentation/cui). Tianyu Cui. USENIX 2021. [[code]](https://github.com/CuiTianyu961030/SiamHAN)
    * [6VecLM: Language Modeling in Vector Space for IPv6 Target Generation](https://link.springer.com/chapter/10.1007%2F978-3-030-67667-4_12). Tianyu Cui. ECML/PKDD 2020. [[code]](https://github.com/CuiTianyu961030/6VecLM)

<!--
# Ethereum
* [A Flexible Sharding Blockchain Protocol Based on Cross-Shard Byzantine Fault Tolerance](https://ieeexplore.ieee.org/abstract/document/10100734). Yizhong Liu. TIFS 2023.
* [Secure and Scalable Cross-Domain Data Sharing in Zero-Trust Cloud-Edge-End Environment Based on Sharding Blockchain](https://ieeexplore.ieee.org/abstract/document/10246351). Yizhong Liu. TDSC 2023.
* [TGC: Transaction Graph Contrast Network for Ethereum Phishing Scam Detection](https://dl.acm.org/doi/abs/10.1145/3627106.3627109). Sijia Li. ACSAC 2023.
* [TTAGN: Temporal transaction aggregation graph network for ethereum phishing scams detection](https://dl.acm.org/doi/abs/10.1145/3485447.3512226). Sijia Li. WWW 2022.
-->

# Teams
* Tsinghua University/China
    * [Ke Xu](http://www.thucsnet.org/xuke.html)
    * [Jiahai Yang](https://nmgroup.tsinghua.edu.cn/yjh/)
    * [Chao Zhang](https://netsec.ccert.edu.cn/chs/people/chaoz/)
    * [Haixin Duan](http://netsec.ccert.edu.cn/people/duanhx/)
    * [Qi Li](https://www.insc.tsinghua.edu.cn/info/1157/2851.htm)
    * [Jianjun Chen](https://www.jianjunchen.com/)
    * [Dan Li](https://www.cs.tsinghua.edu.cn/info/1126/3948.htm)
* Chinese Academy of Sciences, University of Chinese Academy of Sciences/China
    * [Gang Xiong](https://people.ucas.ac.cn/~xionggang) (Institute of Information Engineering)
    * [Kai Chen](https://people.ucas.ac.cn/~kaichen) (Institute of Information Engineering)
    * [Guozhu Meng](https://people.ucas.ac.cn/~gzmeng) (Institute of Information Engineering)
    * [Qingyun Liu](https://people.ucas.ac.cn/~0027674) (Institute of Information Engineering)
    * [Limin Sun](https://people.ucas.ac.cn/~sunlimin) (Institute of Information Engineering)
    * [Zhenyu Li](http://www.ict.ac.cn/sourcedb_2018_ict_cas/cn/jssrck/201111/t20111114_3395505.html) (Institute of Computing Technology)
* Beijing Institute of Technology/China
    * [Liehuang Zhu](https://cs.bit.edu.cn/szdw/jsml/wlkjaqxy/zlh/index.htm)
    * [Meng Shen](https://cst.bit.edu.cn/szdw/jsml/bssds/86728e84066248b0b13bdf04f685817f.htm)
* Xi'an Jiaotong University/China
    * [Xiaohong Guan](https://www.xjtu.edu.cn/jsnr.jsp?wbtreeid=1632&wbwbxjtuteacherid=502)
    * [Chao Shen](https://gr.xjtu.edu.cn/web/cshen)
* Zhejiang University/China
    * [Shouling Ji](https://person.zju.edu.cn/sji#0)
    * [Wenyuan Xu](https://person.zju.edu.cn/wyxu#0)
    * [Meng Luo](https://person.zju.edu.cn/mengluo#0)
    * [Kui Ren](https://person.zju.edu.cn/kuiren)
    * [Fan Zhang](https://person.zju.edu.cn/fanzhang)
* Shanghai Jiao Tong University/China
    * [Guoxing Chen](https://donnod.github.io/)
    * [Haojin Zhu](https://nsec.sjtu.edu.cn/~hjzhu/)
* [Guang Cheng](https://cyber.seu.edu.cn/cg1/list.htm) (Southeast University/China)
* [Fengwei Zhang](https://fengweiz.github.io/) (Southern University of Science and Technology/China)
* [Qian Wang](http://nisplab.whu.edu.cn/people.html) (Wuhan University/China)
* [Min Yang](https://cs.fudan.edu.cn/3e/d7/c25921a278231/page.htm) (Fudan University/China)
* Overseas Teams
    * [Xuemin (Sherman) Shen](https://uwaterloo.ca/scholar/sshen) (University of Waterloo/Canada)
    * [Xiaofeng Wang](https://homes.luddy.indiana.edu/xw7/) (Indiana University Bloomington/United States)
    * [Tao Wang](https://www.cs.sfu.ca/~taowang/) (Simon Fraser University/Canada)
    * [Ivan Martinovic](https://www.cs.ox.ac.uk/people/ivan.martinovic/) (University of Oxford/United Kingdom)
    * [Amir Houmansadr](https://people.cs.umass.edu/~amir/) (University of Massachusetts Amherst/United States)
    * [Giuseppe Aceto](http://wpage.unina.it/giuseppe.aceto/) (Università di Napoli Federico II/Italy)
    * [Thorsten Holz](https://cispa.de/en/research/groups/holz) (CISPA Helmholtz Center for Information Security/Germany)
    * [Mohammad Saidur Rahman](https://www.rahmanmsaidur.com/) (University of Texas at El Paso/United States)
    * [Yue Zhang](https://yue.zyueinfosec.com/) (Drexel University/United States)
    * [Xinyu Xing](http://xinyuxing.org/) (Northwestern University/United States)
    * [Yang Liu](https://personal.ntu.edu.sg/yangliu/) (Nanyang Technological University/Singapore)

# Blogs
## Network Traffic Knowledge
* [Icoding_F2014](https://blog.csdn.net/jmh1996)
* [Malware-Traffic-Analysis](https://www.malware-traffic-analysis.net/)

## Network Traffic Analysis Tool Manual
* [Tshark](https://www.wireshark.org/docs/man-pages/tshark.html)
* [pyshark](https://github.com/KimiNewt/pyshark)
<!--
https://dilidonglong.com/2019/04/26/tshark%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95/
-->

# Tool Libraries and Frameworks
* [flowcontainer](https://github.com/jmhIcoding/flowcontainer)
* [scapy](https://scapy.net/)
* [wireshark](https://www.wireshark.org/)
* [pyshark](https://kiminewt.github.io/pyshark/)
* [Cisco Talos](https://talosintelligence.com/software)
* [Joy](https://github.com/cisco/joy)
* [Proxifier](https://www.proxifier.com/)
* [traffic_classification_utils](https://github.com/jmhIcoding/traffic_classification_utils)

# What's New
**Version 1.0**

> April 15, 2022 

1. Welcome to the Ph.Ds from IIE,CAS.

# Contributors 🌟

Thanks goes to these wonderful people!

<table>
  <tr>
    <td align="center"><a href="https://linwhitehat.github.io/"><img src="https://avatars3.githubusercontent.com/u/20349381?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Xinjie Lin</b></sub></a><br /><a href="#ideas-XinjieLin" title="Ideas, Planning, & Feedback">🎯</a> <a href="https://github.com/linwhitehat/ETA-Resource/commits?author=linwhitehat" title="Documentation">📝</a> <a href="#maintenance-XinjieLin" title="Maintenance">📔</a></td>
    <td align="center"><a href="https://github.com/CuiTianyu961030"><img src="https://avatars.githubusercontent.com/u/43595189?v=4" width="100px;" alt=""/><br /><sub><b>Tianyu Cui</b></sub></a><br /><a href="#ideas-TianyuCui" title="Ideas, Planning, & Feedback">🎯</a> </td>
    <td align="center"><a href="https://github.com/jmhIcoding"><img src="https://avatars.githubusercontent.com/u/19209689?v=4" width="100px;" alt=""/><br /><sub><b>Minghao Jiang</b></sub></a><br /><a href="#ideas-MinghaoJiang" title="Ideas, Planning, & Feedback">🎯</a> </td>
    <td align="center"><a href="https://github.com/GuanZH95"><img src="https://avatars.githubusercontent.com/u/30852909?v=4" width="100px;" alt=""/><br /><sub><b>Zhong Guan</b></sub></a><br /><a href="#ideas-ZhongGuan" title="Ideas, Planning, & Feedback">🎯</a> <a href="https://github.com/linwhitehat/ETA-Resource/commits?author=GuanZH95" title="Documentation">📝</a></td>
    <td align="center"><a href="https://github.com/wayneowen7"><img src="https://avatars.githubusercontent.com/u/29433723?v=4" width="100px;" alt=""/><br /><sub><b>Wei Cai</b></sub></a><br /><a href="#ideas-WeiCai" title="Ideas, Planning, & Feedback">🎯</a> </td>
    <td align="center"><a href="https://github.com/XiyuanZhang971118"><img src="https://avatars.githubusercontent.com/u/155507014?v=4" width="100px;" alt=""/><br /><sub><b>Xiyuan Zhang</b></sub></a><br /><a href="#ideas-XiyuanZhang" title="Ideas, Planning, & Feedback">🎯</a> <a href="https://github.com/linwhitehat/ETA-Resource/commits?author=XiyuanZhang971118" title="Documentation">📝</a></td>
  </tr>
</table>
