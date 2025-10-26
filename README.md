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

<!--
<a href="https://github.com/linwhitehat/ETA-Resource/blob/main/LICENSE">
        <img alt="GitHub" src="https://img.shields.io/github/license/linwhitehat/ETA-Resource.svg?color=green">
    </a>
    <img src="https://img.shields.io/github/stars/linwhitehat/ETA-Resource">
    <img src="https://img.shields.io/github/forks/linwhitehat/ETA-Resource">
-->

<p align="center">
    <img src="https://img.shields.io/badge/License-MIT-brightgreen">
    <img src="https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Flinwhitehat%2FETA-Resource&label=visitor%20%20%20&labelColor=%23697689&countColor=%232ccce4&style=flat">
    <img src="https://img.shields.io/badge/Contributors-13-blue.svg">
</p>

**Note:**
- ⭐ **Please leave a <font color='orange'>STAR</font> if you like this project!** ⭐
- If you find any <font color='red'>incorrect</font> / <font color='red'>inappropriate</font> / <font color='red'>outdated</font> content, please kindly consider opening an issue or a PR. 
- We would greatly appreciate your contribution to this list, and you will appear in the [contributors✨](#contributors-)!

# Content
- [About](#about)
- [Dataset](#datasets)
- [Survey & Benchmark](#survey-and-benchmark)
    - [Survey](#survey)
    - [Benchmark](#benchmark)
- [Encrypted Traffic Analysis](#encrypted-traffic-analysis)
    - [Encrypted Traffic Classification](#encrypted-traffic-classification)
        - [Applied Pre-training/LLMs](#applied-pre-trainingllms)
        - [Applied ML/DL](#applied-machine-learningdeep-learning)
    - [Network Traffic Simulation](#network-traffic-simulation)
        - [Applied Pre-training/LLMs](#applied-ptllms)
        - [Applied ML/DL](#applied-mldl)
    - [Network Intrusion Detection](#network-intrusion-detection)
        - [General Threat Detection](#general-threat-detection)
        - [Malware/C2 Traffic Detection](#malwarec2-traffic-detection)
        - [IoT and Scenario-Specific Detection](#iot-and-scenario-specific-detection)
        - [Black/Grey Market Activity Detection](#blackgrey-market-activity-detection)
    - [WFP and AFP](#wfp-and-afp)
        - [General Fingerprinting](#general-fingerprinting)
        - [Website Fingerprinting](#website-fingerprinting)
        - [App Fingerprinting](#app-fingerprinting)
    - [Generalization and Robustness](#generalization-and-robustness)
    - [Online Methods](#online-methods)
- [Measurement](#measurement)
- [Research Groups](#research-groups)
- [Blogs](#blogs)
- [Tool Libraries and Frameworks](#tool-libraries-and-frameworks)
- [News and Updates](#news-and-updates)
- [Contributors](#contributors-)
<!--
- [Ethereum](#ethereum)
-->

# About
This repository offers a curated collection of research and development resources in the field of encrypted traffic analysis, with an emphasis on representative studies, datasets, and notable research groups.
<!-- This is a current list of resources related to the research and development of encrypted traffic analysis. We comb the field for relevant representative work and related resources, and pay more attention to typical studies and research teams.-->

# Datasets
| Dataset| Description | Year |  Status  |
|--------|-------------|------|----------|
| [Canadian Institute for Cybersecurity Datasets](https://www.unb.ca/cic/datasets/) | IoT, LLM, DNS, IDS, DoS, Darknet, Tor, VPN, Botnet, Malware | – | 🟢&nbsp;Regularly |
| [ANT Datasets](https://ant.isi.edu/datasets/index.html) | Botnet, IoT, DNS, IP Geolocation | – | 🟢&nbsp;Regularly |
| [Information Security and Object Technology Research Lab Datasets](https://onlineacademiccommunity.uvic.ca/isot/datasets/) | IoT, Botnet, Cloud Security | – | 🟢&nbsp;Regularly |
| [VisQUIC](https://github.com/robshahla/VisQUIC) | QUIC Traffic Captured from Different Webpages | 2025 | 🔵&nbsp;New |
| [CipherSpectrum](https://cspectrum.web.cse.unsw.edu.au) | TLS 1.3 Web-Traffic for 40 Domains | 2025 | 🔵&nbsp;New |
| [NETD](https://github.com/linwhitehat/NETD) | Dynamic Non-I.I.D. Encrypted Traffic Dataset | 2025 | 🔵&nbsp;New |
| [MobileTraffic](https://github.com/Abby-ZS/NUDT_MobileTraffic) | 300+ Mobile Apps | 2024 | 🟡&nbsp;No updates |
| [Network Multiflow Fingerprinting Datasets](https://github.com/shashadehuajiang/trace_classifier) | UAV, IoT Device ID, ISD, KWS, SWF | 2023 | 🟡&nbsp;No updates |
| [Itc-Net-Blend-60](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4661706) | Android Apps in Diverse Environments | 2023 | 🟡&nbsp;No updates |
| [AnonProxy2023](https://github.com/MrRobotsAA/AnonProxy2023-Dataset) | Anonymous, Proxy, VPN | 2023 | 🟡&nbsp;No updates |
| [CSTNET-TLS 1.3](https://github.com/linwhitehat/ET-BERT/tree/main/datasets/CSTNET-TLS%201.3) | TLS 1.3 Services | 2022 | 🟡&nbsp;No updates |
| [LFETT2021 Dataset](https://github.com/HoneyPotter-Gzy/LFETT2021-dataset) | Tunnel, Proxy, VPN | 2021 | 🟡&nbsp;No updates |
| [DataCon2021-Encrypted Proxy](https://datacon.qianxin.com/opendata/openpage?resourcesId=10) | Proxy, VPN | 2021 | 🟡&nbsp;No updates |
| [Malware Capture Facility Project](https://www.stratosphereips.org/datasets-overview) | CTU, IoT, Malware, Botnet | 2020 | 🟡&nbsp;No updates |
| [Cross-Platform](https://recon.meddle.mobi/cross-market.html) ([Backup Dataset](https://cloud.tsinghua.edu.cn/f/b00ce0c960114b59b948/)) | iOS and Android Apps | 2019 | 🟡&nbsp;No updates |
| [Network-based Intrusion Detection](https://www.sciencedirect.com/science/article/pii/S016740481930118X) | AWID, Botnet, CIC DoS, CTU, DARPA | 2019 | 🟡&nbsp;No&nbsp;updates |
| [Wangknn-dataset](https://github.com/kdsec/wangknn-dataset) | Tor, Websites | 2018 | 🟡&nbsp;No updates |
| [DLWF](https://github.com/DistriNet/DLWF) | Tor, Websites, Concept Drift, Open World | 2018 | 🟡&nbsp;No updates |
| [Network-Flow-of-QUIC](https://drive.google.com/drive/folders/1cwHhzvaQbi-ap8yfrj2vHyPmUTQhaYOj) | QUIC Services | 2017 | 🟡&nbsp;No updates |

<!--<details>
<summary>
    Datasets for Challenging Tasks
</summary>

* [Canadian Institute for Cybersecurity Datasets](https://www.unb.ca/cic/datasets/) (IoT, LLM, DNS, IDS, DoS, Darknet, Tor, VPN, Botnet, Malware)(Regularly updated)
* [ANT Datasets](https://ant.isi.edu/datasets/index.html) (Botnet, IoT, DNS, IP Geolocation)(Regularly updated)
* [Information Security and Object Technology Research Lab Datasets](https://onlineacademiccommunity.uvic.ca/isot/datasets/) (IoT, Botnet, Cloud Security)(Regularly updated)
* [MobileTraffic](https://github.com/Abby-ZS/NUDT_MobileTraffic) (300+ Mobile Apps)(2024)
* [Network Multiflow Fingerprinting Datasets](https://github.com/shashadehuajiang/trace_classifier) (User Activities (UAV), IoT Device Identification (IDI), Intrusion Detection (ISD), Keyword Searching (KWS), Shadowsocks Website 
Fingerprinting (SWF))(2023)
* [Itc-Net-Blend-60](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4661706) (Android applications in Diverse Environments)(2023)
* [AnonProxy2023](https://github.com/MrRobotsAA/AnonProxy2023-Dataset) (Anonymous, Proxy, VPN)(2023)
* [CSTNET-TLS 1.3](https://drive.google.com/drive/folders/1JSsYmevkxQFanoKOi_i1ooA6pH3s9sDr?usp=sharing) (TLS 1.3 services)(2022)
* [LFETT2021 Dataset](https://github.com/HoneyPotter-Gzy/LFETT2021-dataset) (Tunnel, Proxy, VPN)(2021)
* [DataCon2021-Encrypted Proxy](https://datacon.qianxin.com/opendata/openpage?resourcesId=10) (Proxy, VPN)(2021)
* [Malware Capture Facility Project](https://www.stratosphereips.org/datasets-overview) (CTU, IoT, Malware, Botnet)(2020)
* [Cross-Platform](https://recon.meddle.mobi/cross-market.html) (iOS and Android Apps)(2019)
* [Network-based Intrusion Detection](https://www.sciencedirect.com/science/article/pii/S016740481930118X) (AWID, Botnet, CIC DoS, CICIDS, CIDDS, CTU, DARPA, ISCX, IRSC)(2019)
* [wangknn-dataset](https://github.com/kdsec/wangknn-dataset) (Tor, Websites)(2018)
* [DLWF](https://github.com/DistriNet/DLWF) (Tor, Websites, Concept Drift, Open World)(2018)
* [Network-Flow-of-QUIC](https://drive.google.com/drive/folders/1cwHhzvaQbi-ap8yfrj2vHyPmUTQhaYOj) (QUIC services)(2017)
</details>

<details>
<summary>
    Network Benchmark
</summary>
    
* [NetBench: A Large-Scale and Comprehensive Network Traffic Benchmark Dataset for Foundation Models](https://arxiv.org/abs/2403.10319). [[Data]](https://github.com/WM-JayLab/NetBench)
</details>
-->

# Survey and Benchmark
## Survey
* [Decision-Making Large Language Model for Wireless Communication: A Comprehensive Survey on Key Techniques](https://ieeexplore.ieee.org/abstract/document/11180008). Ning Yang. `IEEE Communications Surveys & Tutorials 2025`.
* [SoK: Decoding the Enigma of Encrypted Network Traffic Classifiers](https://ieeexplore.ieee.org/abstract/document/11023502). Nimesha Wickramasinghe. `S&P 2025`. [[code]](https://github.com/nime-sha256/ntc-enigma)
* [Large Language Model (LLM) for Telecommunications: A Comprehensive Survey on Principles, Key Techniques, and Opportunities](https://doi.org//10.1109/COMST.2024.3465447). Hao Zhou. `IEEE Communications Surveys & Tutorials 2025`.
* [Deep learning and pre-training technology for encrypted traffic classification: A comprehensive review](https://www.sciencedirect.com/science/article/abs/pii/S0925231224012153). Wenqi Dong. `Neurocomputing 2024`.
* [SoK: A Critical Evaluation of Efficient Website Fingerprinting Defenses](https://ieeexplore.ieee.org/document/10179289). Nate Mathews. `S&P 2023`.
* [Machine Learning-Powered Encrypted Network Traffic Analysis: A Comprehensive Survey](https://ieeexplore.ieee.org/document/9896143). Meng Shen. `IEEE Communications Surveys & Tutorials 2023`.
* [Graph Mining for Cybersecurity: A Survey](https://dl.acm.org/doi/10.1145/3610228). Bo Yan. `ACM Transactions on Knowledge Discovery from Data 2023`.
* [Deep Learning for Encrypted Traffic Classification: An Overview](https://ieeexplore.ieee.org/document/8713803/). Shahbaz Rezaei. `IEEE Communications Magazine 2019`.
* [Towards the Deployment of Machine Learning Solutions in Network Traffic Classification: A Systematic Survey](https://ieeexplore.ieee.org/document/8543584). Fannia Pacheco. `IEEE Communications Surveys & Tutorials 2019`.
* [Deep Learning in Mobile and Wireless Networking: A Survey](https://ieeexplore.ieee.org/document/8666641). Chaoyun Zhang. `IEEE Communications Surveys & Tutorials 2019`.
## Benchmark
* [The Digital Cybersecurity Expert: How Far Have We Come?](https://arxiv.org/abs/2504.11783). Dawei Wang. `S&P 2025`. [[Report]](https://mp.weixin.qq.com/s/0G0iJue6yJval7sYAmtFEg) [[BenchMark]](https://github.com/NASP-THU/CSEBenchmark)
* [Demystifying Network Foundation Models](https://arxiv.org/abs/2509.23089). Sylee Beltiukov. `NeurIPS 2025`. [[BenchMark]](https://github.com/maybe-hello-world/demystifying-networks)
* [SECURE: Benchmarking Large Language Models for Cybersecurity](https://ieeexplore.ieee.org/document/10917682). Dipkamal Bhusal. `ACSAC 2024`. [[BenchMark]](https://github.com/aiforsec/SECURE)
* [CTIBench: A Benchmark for Evaluating LLMs in Cyber Threat Intelligence](https://proceedings.neurips.cc/paper_files/paper/2024/file/5acd3c628aa1819fbf07c39ef73e7285-Paper-Datasets_and_Benchmarks_Track.pdf#:~:text=To%20bridge%20this%20gap%2C%20we,bench). Md Tanvirul Alam. `NeurIPS 2024`. [[Evaluation]](https://github.com/aiforsec/cti-bench) [[BenchMark]](https://huggingface.co/datasets/AI4Sec/cti-bench)
* [NetBench: A Large-Scale and Comprehensive Network Traffic Benchmark Dataset for Foundation Models](https://arxiv.org/abs/2403.10319). Qian Chen. `FMSys 2024`. [[Dataset]](https://github.com/WM-JayLab/NetBench)

# Encrypted Traffic Analysis
## Encrypted Traffic Classification
### Applied Pre-training/LLMs
* [MOTA: Mixture Of Traffic Agents for Robust Network Traffic Classification](https://www.researchgate.net/publication/395505247_MOTA_Mixture_of_Traffic_Agents_for_Robust_Network_Traffic_Classification). Shaowei Li. `IWQoS 2025`.
* [TraGe: A Generic Packet Representation for Traffic Classification Based on Header-Payload Differences](https://arxiv.org/abs/2506.14151). Chungang Lin. `IWQoS 2025`.
* [Swallow: A Transfer-Robust Website Fingerprinting Attack via Consistent Feature Learning](). Meng Shen. `CCS 2025`. [[code]](https://github.com/wujinhe0814/Swallow)
* [MM4flow: A Pre-trained Multi-modal Model for Versatile Network Traffic Analysis](). Luming Yang. `CCS 2025`.
* [MIETT: Multi-Instance Encrypted Traffic Transformer for Encrypted Traffic Classification](https://arxiv.org/abs/2412.15306). Xuyang Chen and Lu Han. `AAAI 2025`.
* [TrafficFormer: An Efficient Pre-trained Model for Traffic Data](https://www.computer.org/csdl/proceedings-article/sp/2025/223600a102/22K50xTq93y). Guangmeng Zhou. `S&P 2025`. [[code]](https://github.com/IDP-code/TrafficFormer)
* [Ptu: Pre-Trained Model for Network Traffic Understanding](https://ieeexplore.ieee.org/document/10858503). Lingfeng Peng. `ICNP 2024`.
* [NetMamba: Efficient Network Traffic Classification via Pre-training Unidirectional Mamba](https://arxiv.org/abs/2405.11449). Tongze Wang. `ICNP 2024`. [[code]](https://github.com/wangtz19/NetMamba)
* [Flow-MAE: Leveraging Masked AutoEncoder for Accurate, Efficient and Robust Malicious Traffic Classification](https://dl.acm.org/doi/10.1145/3607199.3607206#core-collateral-purchase-access). Zijun Hang. `RAID 2023`. [[code]](https://github.com/NLear/Flow-MAE)
* [Listen to Minority: Encrypted Traffic Classification for Class Imbalance with Contrastive Pre-Training](https://ieeexplore.ieee.org/abstract/document/10287449). Xiang Li. `SECON 2023`.
* [Yet Another Traffic Classifier: A Masked Autoencoder Based Traffic Transformer with Multi-Level Flow Representation](https://ojs.aaai.org/index.php/AAAI/article/view/25674). Ruijie Zhao. `AAAI 2023`. [[code]](https://github.com/NSSL-SJTU/YaTC)
* [MT-FlowFormer: A Semi-Supervised Flow Transformer for Encrypted Traffic Classification](https://dl.acm.org/doi/10.1145/3534678.3539314). Ruijie Zhao. `KDD 2022`.
* [ET-BERT: A Contextualized Datagram Representation with Pre-training Transformers for Encrypted Traffic Classification](https://dl.acm.org/doi/abs/10.1145/3485447.3512217). Xinjie Lin. `WWW 2022`. [[code]](https://github.com/linwhitehat/et-bert) [[Reproduce]](https://gitee.com/xxdxxdxxd/et-bert/blob/master/README.md)
### Applied Machine Learning/Deep Learning
* [Revolutionizing Encrypted Traffic Classification with MH-Net: A Multi-View Heterogeneous Graph Model](https://arxiv.org/abs/2501.03279). Haozhen Zhang. `AAAI 2025`. [[code]](https://github.com/ViktorAxelsen/MH-Net)
* [FlowMiner: A Powerful Model Based on Flow Correlation Mining for Encrypted Traffic Classification](). Hongbo Xu. `INFOCOM 2025`.
* [TFE-GNN: A Temporal Fusion Encoder Using Graph Neural Networks for Fine-grained Encrypted Trafic Classification](https://dl.acm.org/doi/abs/10.1145/3543507.3583227). Haozhen Zhang. `WWW 2023`. [[code]](https://github.com/ViktorAxelsen/TFE-GNN)
* [An Input-Agnostic Hierarchical Deep Learning Framework for Traffic Fingerprinting](https://www.usenix.org/conference/usenixsecurity23/presentation/qu). Jian Qu. `USENIX Security 2023`. [[code]](https://github.com/shashadehuajiang/trace_classifier/tree/main)
* [Packet Representation Learning for Traffic Classification](https://dl.acm.org/doi/10.1145/3534678.3539085). Xuying Meng. `KDD 2022`. [[code]](https://github.com/ict-net/PacRep)
* [Enabling Efficient Flow Classification for ML-based Network Security Applications](https://www.ndss-symposium.org/wp-content/uploads/ndss2021_7C-2_24067_paper.pdf). Diogo Barradas. `NDSS 2021`. [[code]](https://github.com/dmbb/FlowLens)
* [FS-Net: A Flow Sequence Network For Encrypted Traffic Classification](https://ieeexplore.ieee.org/document/8737507). Chang Liu. `INFOCOM 2019`. [[code]](https://github.com/WSPTTH/FS-Net)
* [MaMPF: Encrypted Traffic Classification Based on Multi-Attribute Markov Probability Fingerprints](https://ieeexplore.ieee.org/abstract/document/8624124).  Chang Liu. `IWQoS 2018`. [[code]](https://github.com/WSPTTH/MaMPF)

## Network Traffic Simulation
### Applied PT/LLMs
* [Resolving Packets from Counters: Enabling Multi-scale Network Traffic Super Resolution via Composable Large Traffic Model](https://www.usenix.org/conference/nsdi25/presentation/wang-xizheng-resolving). Xizheng Wang. `NSDI 2025`. [[code]](https://github.com/wxzisk/ZoomSynth_NSDI2025)
* [NetLLM: Adapting Large Language Models for Networking](https://dl.acm.org/doi/abs/10.1145/3651890.3672268). Duo Wu. `SIGCOMM 2024`. [[code]](https://github.com/duowuyms/NetLLM)
* [NetDiffusion: Network Data Augmentation Through Protocol-Constrained Traffic Generation](https://dl.acm.org/doi/10.1145/3639037). Xi Jiang. `SIGMETRICS 2023`. [[code](https://github.com/noise-lab/NetDiffusion_Generator)]
### Applied ML/DL
* [Datacenter Network Deserves Be!er Traffic Models](https://conferences.sigcomm.org/hotnets/2023/papers/hotnets23_huang.pdf). Sijiang Huang. `HotNets 2023`.
* [Practical GAN-based synthetic IP header trace generation using NetShare](https://dl.acm.org/doi/10.1145/3544216.3544251). Yucheng Yin. `SIGCOMM 2022`. [[code](https://github.com/netsharecmu/NetShare)]

## Network Intrusion Detection
### General Threat Detection
* [Robust Detection of Malicious Encrypted Traffic via Contrastive Learning](https://ieeexplore.ieee.org/abstract/document/10964328). Meng Shen. `TIFS 2025`.
* [Trident: A Universal Framework for Fine-Grained and Class-Incremental Unknown Traffic Detection](https://dl.acm.org/doi/10.1145/3589334.3645407). Secbrain. `WWW 2024`. [[code]](https://github.com/Secbrain/Trident/)
* [Mateen: Adaptive Ensemble Learning for Network Anomaly Detection](https://dl.acm.org/doi/10.1145/3678890.3678901). Fahad Alotaibi. `RAID 2024`. [[code]](https://github.com/ICL-ml4csec/Mateen/)
* [AOC-IDS: Autonomous Online Framework with Contrastive Learning for Intrusion Detection](https://ieeexplore.ieee.org/document/10621346). Xinchen Zhang. `INFOCOM 2024`. [[code]](https://github.com/xinchen930/AOC-IDS)
* [Early Network Intrusion Detection Enabled by Attention Mechanisms and RNNs](https://doi.org/10.1109/TIFS.2024.3441862). Taki Eddine Toufik Djaidja. `TIFS 2024`.
* [TMG-GAN: Generative Adversarial Networks-Based Imbalanced Learning for Network Intrusion Detection](https://dl.acm.org/doi/10.1109/TIFS.2023.3331240). Hongwei Ding. `TIFS 2024`.
* [Network intrusion detection based on n-gram frequency and time-aware transformer](https://www.sciencedirect.com/science/article/pii/S0167404823000810?via%3Dihub). Xueying Han. `Computer Security 2023`.
* [Encrypted Malware Traffic Detection via Graph-based Network Analysis](https://dl.acm.org/doi/10.1145/3545948.3545983). Zhuoqun Fu. `RAID 2022`.
* [Interactive Anomaly Detection in Dynamic Communication Networks](https://ieeexplore.ieee.org/abstract/document/9494106). Xuying Meng. `ToN 2021`. [[code]](https://github.com/ict-net/HADDN)

### Malware/C2 Traffic Detection
* [Wedjat: Detecting Sophisticated Evasion Attacks via Real-time Causal Analysis](http://www.thucsnet.com/wp-content/papers/li_gao_kdd2025.pdf). Li Gao. `KDD 2025`.
* [PETNet: Plaintext-aware encrypted traffic detection network for identifying Cobalt Strike HTTPS traffics](https://www.sciencedirect.com/science/article/pii/S1389128623005650). Xiaodu Yang. `Computer Networks 2024`. [[code]](https://github.com/CN-PETNet/PETNet)
* [Detecting Tunneled Flooding Traffic via Deep Semantic Analysis of Packet Length Patterns](https://dl.acm.org/doi/abs/10.1145/3658644.3670353). Chuanpu Fu. `CCS 2024`. [[code]](https://github.com/fuchuanpu/Exosphere)
* [Point Cloud Analysis for ML-Based Malicious Traffic Detection: Reducing Majorities of False Positive Alarms](https://dl.acm.org/doi/10.1145/3576915.3616631). Chuanpu Fu. `CCS 2023`. [[code]](https://github.com/fuchuanpu/pVoxel)
* [Detecting Unknown Encrypted Malicious Traffic in Real Time via Flow Interaction Graph Analysis](https://www.ndss-symposium.org/wp-content/uploads/2023/02/ndss2023_s80_paper.pdf). Chuanpu Fu. `NDSS 2023`. [[code]](https://github.com/fuchuanpu/HyperVision)

### IoT and Scenario-Specific Detection
* IoT Malicious Traffic Detection
    * [HorusEye: A Realtime IoT Malicious Traffic Detection Framework using Programmable Switches](https://www.usenix.org/conference/usenixsecurity23/presentation/dong-yutao). Yutao Dong. `USENIX Security 2023`.
* Vehicle Network (IoV) Malicious Traffic Detection
    * [Cyber Security Framework for Vehicular Network Based on a Hierarchical Game](https://ieeexplore.ieee.org/document/8598790). Hichem Sedjelmaci. `IEEE Transactions on Emerging Topics in Computing 2021`.

### Black/Grey Market Activity Detection
**Illegal Traffic Identification**
* Gambling Detection
    * [Let gambling hide nowhere: Detecting illegal mobile gambling apps via heterogeneous graph-based encrypted traffic analysis](https://www.sciencedirect.com/science/article/pii/S1389128624001105). Zheyuan Gu. `Computer Networks 2024`.
    * [Gambling Domain Name Recognition via Certificate and Textual Analysis](https://academic.oup.com/comjnl/article/66/8/1829/6570684). GuoYing Sun. `The Computer Journal 2023`.
    * [Analyzing Ground-Truth Data of Mobile Gambling Scams](https://ieeexplore.ieee.org/abstract/document/9833665). Geng Hong. `Symposium on Security and Privacy (S&P) 2022`.

## WFP and AFP
### General Fingerprinting
* [HOLMES & WATSON: A Robust and Lightweight HTTPS Website Fingerprinting through HTTP Version Parallelism](https://dl.acm.org/doi/10.1145/3696410.3714578). Yifei Cheng. `WWW 2025`.
* [Nüwa: Enhancing Network Traffic Analysis With Pre-Trained Side-Channel Feature Imputation](https://ieeexplore.ieee.org/abstract/document/11071392). Faqi Zhao. `ToN 2025`.
* [DE-GNN: Dual embedding with graph neural network for fine-grained encrypted traffic classification](https://www.sciencedirect.com/science/article/pii/S1389128624002044). Xinbo Han. `Computer Networks 2024`.
* [Seeing Traffic Paths: Encrypted Traffic Classification With Path Signature Features](https://ieeexplore.ieee.org/document/9786755). Shijie Xu. `TIFS 2022`.
* [A Novel Multimodal Deep Learning Framework for Encrypted Traffic Classification](https://ieeexplore.ieee.org/document/9931999). Peng Lin. `ToN 2022`.
* [Accurate Decentralized Application Identification via Encrypted Traffic Analysis Using Graph Neural Networks](https://ieeexplore.ieee.org/document/9319399).  Meng Shen. `TIFS 2021`.
* [Classifying encrypted traffic using adaptive fingerprints with multi-level attributes](https://link.springer.com/article/10.1007%2Fs11280-021-00940-0). Chang Liu. `WWW Journal 2021`.
* [Fine-Grained Webpage Fingerprinting Using Only Packet Length Information of Encrypted Traffic](https://ieeexplore.ieee.org/document/9305740). Meng Shen. `TIFS 2020`.
* [CETAnalytics: Comprehensive effective traffic information analytics for encrypted traffic classification](https://www.sciencedirect.com/science/article/pii/S1389128619309466). Cong Dong. `Computer Networks 2020`.
### Website Fingerprinting
* Tunnel and VPN
    * [Fingerprinting Obfuscated Proxy Traffic with Encapsulated TLS Handshakes](https://www.usenix.org/conference/usenixsecurity24/presentation/xue-fingerprinting). Diwen Xue. `USENIX Security 2024`.
    * [ProxyKiller: An Anonymous Proxy Traffic Attack Model Based on Traffic Behavior Graphs](https://link.springer.com/chapter/10.1007/978-3-031-70890-9_9#Tab4). Hongbo Xu. `ESORICS 2024`.
    * [VPNSniffer: Identifying VPN Servers Through Graph-Represented Behaviors](https://dl.acm.org/doi/10.1145/3589334.3645552). Chenxu Wang. `WWW 2024`.
    * [Causality Correlation and Context Learning Aided  Robust Lightweight Multi-Tab Website  Fingerprinting Over Encrypted Tunnel](https://ieeexplore.ieee.org/abstract/document/10621235). Siyang Chen. `INFOCOM 2024`. [[code]](https://github.com/chenxiailian/robustweb) [[data]](https://drive.google.com/file/d/1_NvHBp4Z96UuWw5LwEEcb-WfMrOrEoDP/view?usp=drive_linkS)
    * [Website Fingerprinting on Encrypted Proxies: A Flow-Context-Aware Approach and Countermeasures](https://ieeexplore.ieee.org/abstract/document/10345509). Xiaobo Ma. `ToN 2024`. [[code]](https://github.com/sevensmith/context-aware-wfp)
    * [Context-aware Website Fingerprinting over Encrypted Proxies](https://ieeexplore.ieee.org/abstract/document/9488676). Xiaobo Ma. `INFOCOM 2021`.
* Tor
    * [Beyond Single Tabs: A Transformative Few-Shot Approach to Multi-Tab Website Fingerprinting Attacks](https://dl.acm.org/doi/10.1145/3696410.3714811). Wenwen Meng. `WWW 2025`. [[code]](https://github.com/WW-Meng/FMWF)
    * [Enhancing Search Privacy on Tor: Advanced Deep Keyword Fingerprinting Attacks and BurstGuard Defense](https://dl.acm.org/doi/abs/10.1145/3708821.3733914). Chaiwon Hwang. `ASIA CCS 2025`.
    * [Stop, Don’t Click Here Anymore: Boosting Website Fingerprinting By Considering Sets of Subpages](https://www.usenix.org/conference/usenixsecurity24/presentation/mitseva). Mitseva and Panchenko. `Usenix Security 2024`. 
    * [Robust and Reliable Early-Stage Website Fingerprinting Attacks via Spatial-Temporal Distribution Analysis](https://arxiv.org/pdf/2407.00918). Xinhao Deng. `CCS 2024`. [[code]](https://github.com/Xinhao-Deng/Website-Fingerprinting-Library)
    * [Towards Fine-Grained Webpage Fingerprinting at Scale](https://dl.acm.org/doi/abs/10.1145/3658644.3690211). Xiyuan Zhao and Xinhao Deng. `CCS 2024`. [[code]](https://zenodo.org/records/13383332)
    * [On Precisely Detecting Censorship Circumvention in Real-World Networks](https://www.ndss-symposium.org/ndss-paper/on-precisely-detecting-censorship-circumvention-in-real-world-networks/). Ryan Wails. `NDSS 2024`.
    * [HSDirSniper: A New Attack Exploiting Vulnerabilities in Tor's Hidden Service Directories](https://dl.acm.org/doi/10.1145/3589334.3645591). Qingfeng Zhang. `WWW 2024`.
    * [Towards Robust Multi-tab Website Fingerprinting](https://arxiv.org/pdf/2501.12622). Xinhao Deng. `S&P 2023`. [[code]](https://github.com/Xinhao-Deng/Multitab-WF-Datasets)
    * [Realistic Website Fingerprinting By Augmenting Network Trace](https://arxiv.org/pdf/2309.10147). Alireza Bahramali. `CCS 2023`. [[code]](https://github.com/SPIN-UMass/Realistic-Website-Fingerprinting-By-Augmenting-Network-Traces)
    * [Transformer-based Model for Multi-tab Website Fingerprinting Attack](https://dl.acm.org/doi/abs/10.1145/3576915.3623107). Zhaoxin Jin. `CCS 2023`. [[code]](https://github.com/jzx-bupt/TMWF)
    * [Online Website Fingerprinting: Evaluating Website Fingerprinting Attacks on Tor in the Real World](https://www.usenix.org/conference/usenixsecurity22/presentation/cherubin). Giovanni Cherubin. `USENIX Security 2022`.
    * [Adaptive Fingerprinting:Website Fingerprinting over Few Encrypted Traffic](https://dl.acm.org/doi/10.1145/3422337.3447835). Chenggang Wang. `CODASPY 2021`.
    * [BAPM: Block Attention Profiling Model for Multi-tab Website Fingerprinting Attacks on Tor](https://dl.acm.org/doi/10.1145/3485832.3485891). Zhong Guan. `ACSAC 2021`.
    * [Triplet Fingerprinting: More Practical and Portable Website Fingerprinting with N-shot Learning](https://dl.acm.org/doi/10.1145/3319535.3354217). Payap Sirinam. `CCS 2019`. [[code]](https://github.com/triplet-fingerprinting/tf)
    * [Tik-Tok: The Utility of Packet Timing in Website Fingerprinting Attacks](https://petsymposium.org/popets/2020/popets-2020-0043.pdf). Mohammad Saidur Rahman. `PETS 2019`. [[code]](https://github.com/msrocean/Tik_Tok)
    * [Deep Fingerprinting: Undermining Website Fingerprinting Defenses with Deep Learning](https://dl.acm.org/doi/abs/10.1145/3243734.3243768). Payap Sirinam. `CCS 2018`. [[code]](https://github.com/deep-fingerprinting/df)
    * [Automated Website Fingerprinting through Deep Learning](https://tor-wf-dl.distrinet-research.be/Rimmer2018-DLWF.pdf). Vera Rimmer. `NDSS 2018`. [[code]](https://github.com/DistriNet/DLWF)
### App Fingerprinting
* Tunnel and VPN
    * [DecETT: Accurate App Fingerprinting Under Encrypted Tunnels via Dual Decouple-based Semantic Enhancement](https://openreview.net/forum?id=y5tQ9BX5NW#discussion). Zheyuan Gu. `WWW 2025`. [[code]](https://github.com/DecETT/DecETT)
    * [AppSniffer: Towards Robust Mobile App Fingerprinting Against VPN](https://dl.acm.org/doi/10.1145/3543507.3583473). Sanghak Oh. `WWW 2023`. [[code]](https://github.com/network-traffic/AppSniffer)
* Mobile App
    * [Ultimate Encrypted Traffic Feature Engineering: HTTPS Encrypted Traffic Classification Using Restored Application Data Unit Length](https://ieeexplore.ieee.org/abstract/document/11184470/keywords#keywords). Zihan Chen. `TDSC 2025`.
    * [A novel approach for application classification with encrypted traffic using BERT and packet headers](https://www.sciencedirect.com/science/article/pii/S1389128624005796). Jaehak Yu. `Computer Networks 2024`.
    * [Packet-Level Open-World App Fingerprinting on Wireless Traffic](https://www.ndss-symposium.org/ndss-paper/auto-draft-218/). Jianfeng Li. `NDSS 2022`. [[code]](https://github.com/jflixjtu/PacketPrint/tree/main)
    * [FlowPrint: Semi-Supervised Mobile-App Fingerprinting on Encrypted Network Traffic](https://www.ndss-symposium.org/wp-content/uploads/2020/02/24412.pdf). Thijs van Ede. `NDSS 2020`. [[code]](https://github.com/Thijsvanede/FlowPrint)
    * [Robust Smartphone App Identification via Encrypted Network Traffic Analysis](https://ieeexplore.ieee.org/document/8006282). Vincent F. Taylor. `IEEE Transactions on Information Forensics and Security (TIFS) 2018`. [[code]](https://github.com/vftaylor/appscanner)
    * [AppScanner: Automatic Fingerprinting of Smartphone Apps from Encrypted Network Traffic](https://ieeexplore.ieee.org/abstract/document/7467370). Vincent F. Taylor. `Euro S&P 2016`. [[code]](https://github.com/vftaylor/appscanner)
    * [Adaptive encrypted traffic fingerprinting with bi-directional dependence](https://dl.acm.org/doi/abs/10.1145/2991079.2991123). Khaled Al-Naami. `ACSAC 2016`. [[code]](https://github.com/khaled-alnaami/NetworkTrafficFingerprinting)
* Streaming Media
    * [JumpDASH: LLM-Based Content Perception for Intelligent Jumping DASH in Mobile Adaptive Video Streaming](https://ieeexplore.ieee.org/document/11216135). Hanling Wang. `ToN 2025`.
    * [PPVF: An Efficient Privacy-Preserving Online Video Fetching Framework With Correlated Differential Privacy](https://ieeexplore.ieee.org/document/11205328). Xianzhi Zhang. `ToN 2025`.
    * [Dive into streaming: efficient identification of encrypted dynamic DASH video traffic](https://link.springer.com/article/10.1007/s11432-024-4474-6). Xiyuan Zhang. `SCIS 2026`.
    * [Endangered Privacy: Large-Scale Monitoring of Video Streaming Services](https://www.usenix.org/conference/usenixsecurity25/presentation/bjorklund). Martin Björklund. `USENIX Security 2025`.
    * [TorVIA A Novel Encrypted Video Identification Method Based on Tor Transmission Characteristics](https://www.sciencedirect.com/science/article/abs/pii/S1389128625005584). Juncheng Lu. `Computer Networks 2025`.
    * [The Analysis of Encrypted Video Stream Based on Low-dimensional Embedding Method](https://ieeexplore.ieee.org/document/10793092). Luming Yang. `TIFS 2024`.
    * [Zenith: Real-time Identification of DASH Encrypted Video Traffic with Distortion](https://dl.acm.org/doi/10.1145/3664647.3680695). Weitao Tang. `MM 2024`.
    * [Breaking Through the Diversity: Encrypted Video Identification Attack Based on QUIC Features](https://link.springer.com/chapter/10.1007/978-3-031-70903-6_9#author-information). Nan Hu. `ESORICS 2024`.
    * [Traffic spills the beans: A robust video identification attack against YouTube](https://www.sciencedirect.com/science/article/abs/pii/S0167404823005333). Xiyuan Zhang. `ComSec 2024`.
    * [EVS2vec: A Low-dimensional Embedding Method for Encrypted Video Stream Analysis](https://ieeexplore.ieee.org/document/10287432). Luming Yang. `SECON 2023`
    * [Walls Have Ears: Traffic-based Side-channel Attack in Video Streaming](https://ieeexplore.ieee.org/abstract/document/8486211). Jiaxi Gu. `IEEE INFOCOM 2018`.
* LLMs Privacy Analysis
    * [What Was Your Prompt? A Remote Keylogging Attack on AI Assistants](https://www.usenix.org/conference/usenixsecurity24/presentation/weiss). Roy Weiss. `USENIX Security 2024`. [[code]](https://github.com/royweiss1/GPT_Keylogger)

## Generalization and Robustness
* Out-of-Distribution
    * [SnifferDog: Comprehensively Learning Heterogeneous Features of Network Traffic to Identify Malicious Flows](https://ieeexplore.ieee.org/abstract/document/11202220/keywords#keywords). Xi Luo. `TIFS 2025`.
    * [Respond to Change with Constancy: Instruction-tuning with LLM for Non-I.I.D. Network Traffic Classification](https://doi.org/10.1109/TIFS.2025.3574971). Xinjie Lin. `TIFS 2025`.
    * [FG-SAT: Efficient Flow Graph for Encrypted Traffic Classification under Environment Shifts](https://ieeexplore.ieee.org/abstract/document/11007150). Susu Cui. `TIFS 2025`.
    * [Facing Anomalies Head-On: Network Traffic Anomaly Detection via Uncertainty-Inspired Inter-Sample Differences](https://openreview.net/forum?id=hcXmL63aOJ#discussion). Xinglin Lian. `WWW 2025`.
    * [CD-Net: Robust mobile traffic classification against apps updating](https://www.sciencedirect.com/science/article/abs/pii/S0167404824005200). Yanan Chen. `ComSec 2025`.
    * [Zero-relabelling mobile-app identification over drifted encrypted network traffic](https://doi.org/10.1016/j.comnet.2023.109728). Minghao Jiang. `Computer Networks 2023`.
    * [Anomaly Detection in the Open World: Normality Shift Detection, Explanation, and Adaptation](https://www.ndss-symposium.org/ndss-paper/anomaly-detection-in-the-open-world-normality-shift-detection-explanation-and-adaptation/). Dongqi Han. `NDSS 2023`. [[code]](https://github.com/dongtsi/OWAD)
    * [Accurate mobile-app fingerprinting using flow-level relationship with graph neural networks](https://www.sciencedirect.com/science/article/pii/S1389128622003577). Minghao Jiang. `Computer Networks 2022`.
    * [CADE: Detecting and Explaining Concept Drift Samples for Security Applications](https://www.usenix.org/conference/usenixsecurity21/presentation/yang-limin). Dongqi Han. `USENIX Security 2021`. [[code]](https://github.com/whyisyoung/CADE)
* Few-shot/Zero-shot
    * [Low-Quality Training Data Only? A Robust Framework for Detecting Encrypted Malicious Network Traffic](https://www.ndss-symposium.org/ndss-paper/low-quality-training-data-only-a-robust-framework-for-detecting-encrypted-malicious-network-traffic/). Yuqi Qing. `NDSS 2024`. [[code]](https://github.com/XXnormal/RAPIER)
    * [CETP: A Novel Semi-Supervised Framework Based on Contrastive Pre-Training for Imbalanced Encrypted Traffic Classification](https://www.sciencedirect.com/science/article/abs/pii/S0167404824001949). Xinjie Lin. `Computers & Security (ComSec) 2024`.
    * [Few-shot encrypted traffic classification via multi-task representation enhanced meta-learning](https://www.sciencedirect.com/science/article/pii/S1389128623001767). Chen Yang. `Computer Networks 2023`.
    * [Triplet Fingerprinting: More Practical and Portable Website Fingerprinting with N-shot Learning](https://dl.acm.org/doi/abs/10.1145/3319535.3354217). Payap Sirinam. `CCS 2019`. [[code]](https://github.com/triplet-fingerprinting/tf) (N-shot Learning)
* Open-set
    * [Reliable Open-Set Network Traﬃc Classification](https://ieeexplore.ieee.org/abstract/document/10900396). Xueman Wang. `TIFS 2025`.
    * [TrafficGPT: An LLM Approach for Open-Set Encrypted Traffic Classification](https://dl.acm.org/doi/abs/10.1145/3674213.3674217). Yasod Ginige. `AINTEC 2024`. [[code]](https://github.com/YasodGinige/TrafficGPT)
    * [Knowing the unknowns: Network traffic detection with open-set semi-supervised learning](https://www.sciencedirect.com/science/article/abs/pii/S1389128624004626). Rui Chen. `Computer Networks 2024`.
    * [Identifying malicious traffic under concept drift based on intraclass consistency enhanced variational autoencoder](http://scis.scichina.com/en/2024/182302.pdf). Xiang Luo. `SCIENCE CHINA Information Sciences (SCIS) 2024`.
    * [Robust open-set classification for encrypted traffic fingerprinting](https://www.sciencedirect.com/science/article/pii/S138912862300436X). Thilini Dahanayaka. `Computer Networks 2023`.
    * [Autonomous Unknown-Application Filtering and Labeling for DL-based Traffic Classifier Update](https://ieeexplore.ieee.org/abstract/document/9155292). Jielun Zhang. `INFOCOM 2020`
* Defense and Adversarial Techniques
    * [Robustness Matters: Pre-Training Can Enhance the Performance of Encrypted Traffic Analysis](https://ieeexplore.ieee.org/abstract/document/11177602). Luming Yang. `TIFS 2025`.[[code]](https://github.com/Shangshu-LAB/BERT-ps)
    * [CertTA: Certified Robustness Made Practical for Learning-Based Traffic Analysis](https://www.usenix.org/conference/usenixsecurity25/presentation/yan-jinzhu). Jinzhu Yan. `USENIX Security 2025`. [[code]](https://github.com/InspiringGroup-Lab/CertTA) [[Zenodo]](https://doi.org/10.5281/zenodo.15580292)
    * [AdvTG: An Adversarial Traffic Generation Framework to Deceive DL-Based Malicious Traffic Detection Models](https://openreview.net/forum?id=sYZvdIh9ro#discussion). Peishuai Sun. `WWW 2025`. [[code]](https://github.com/TrafficDetection-art/AdvTG)
    * [TrafCL: Robust Encrypted Malicious Traffic Detection via Contrastive Learning](https://dl.acm.org/doi/abs/10.1145/3627673.3679839). Xiaodu Yang. `CIKM 2024`.
    * [MCRe: A Unified Framework for Handling Malicious Traffic With Noise Labels Based on Multidimensional Constraint Representation](https://dl.acm.org/doi/10.1109/TIFS.2023.3318962). Qingjun Yuan. `TIFS 2024`.
    * [Real-Time Website Fingerprinting Defense via Traffic Cluster Anonymization](https://www.computer.org/csdl/proceedings-article/sp/2024/313000a263/1WPcZnZILHa). Meng Shen. `S&P 2024`.
    * [Defending Against Deep Learning-Based Traffic Fingerprinting Attacks With Adversarial Examples](https://dl.acm.org/doi/abs/10.1145/3698591). Blake Hayden. `ACM Transactions on Privacy and Security (TOPS) 2024`.
    * [BARS: Local Robustness Certification for Deep Learning based Traffic Analysis Systems](https://www.ndss-symposium.org/ndss-paper/bars-local-robustness-certification-for-deep-learning-based-traffic-analysis-systems/#:~:text=Deep%20learning%20,based%20traffic%20analysis%20systems%20based). Kai Wang. `NDSS 2023`.
    * [Prism: Real-Time Privacy Protection Against Temporal Network Traffic Analyzers](https://ieeexplore.ieee.org/document/10103708). Wenhao Li. `TIFS 2023`.
    * [Subverting Website Fingerprinting Defenses with Robust Traffic Representation](https://www.usenix.org/conference/usenixsecurity23/presentation/shen-meng). Meng Shen. `USENIX Security 2023`.
    * [Rosetta: Enabling Robust TLS Encrypted Traffic Classification in Diverse Network Environments with TCP-Aware Traffic Augmentation](https://www.usenix.org/conference/usenixsecurity23/presentation/xie). Renjie Xie. `USENIX Security 2023`. [[code]](https://github.com/sunskyXX/Rosetta)
* Explanatory Analysis
    * [The Sweet Danger of Sugar: Debunking Representation Learning for Encrypted Traffic Classification](https://dl.acm.org/doi/10.1145/3718958.3750498). Yuqi Zhao. `SIGCOMM 2025`.
    * [Explainable Anomaly Detection in Network Traffic Using Normalizing Flows](https://xplorestaging.ieee.org/document/11201273). Lior Shafir. `ToN 2025`.
    * [Understanding Web Fingerprinting with a Protocol-Centric Approach](https://dl.acm.org/doi/10.1145/3678890.3678910). Bogdan Cebere. `RAID 2024`. [[code]](https://github.com/bcebere/Understanding-and-Explaining-Web-Fingerprinting-with-a-Protocol-Centric-Approach)
    * [GEAD: Rules Refine the Riddle: Global Explanation for Deep Learning-Based Anomaly Detection in Security Applications](https://dl.acm.org/doi/10.1145/3658644.3670375). Dongqi Han. `CCS 2024`. [[code]](https://github.com/dongtsi/GEAD)
    * [Towards Real-Time Intrusion Detection with Explainable AI-Based Detector](https://dl.acm.org/doi/10.1145/3658644.3691410). Wenhao Li. `CCS Poster 2024`.
    * [xNIDS: Explaining Deep Learning-based Network Intrusion Detection Systems for Active Intrusion Responses](https://www.usenix.org/conference/usenixsecurity23/presentation/wei-feng). Feng Wei. `USENIX Security 2023`. [[code]](https://github.com/CactiLab/code-xNIDS)
    * [Towards Understanding Alerts raised by Unsupervised Network Intrusion Detection Systems](https://dl.acm.org/doi/10.1145/3607199.3607247). Maxime Lanvin. `RAID 2023`.
    * [AI/ML for Network Security: The Emperor has no Clothes](https://dl.acm.org/doi/10.1145/3548606.3560609). Arthur S. Jacobs. `CCS 2022`. [[code]](https://github.com/TrusteeML/trustee)
<!-- * [Explaining Deep Learning Models for Per-packet Encrypted Network Traffic Classification](https://ant.isi.edu/~hardaker/papers/Explaining_Deep_Learning_Models_for_Per-packet_Encrypted_Network_Traffic_Classification.pdf#:~:text=we%20propose%20a%20methodology%20to,directions%20toward%20optimizing%20model%20performance). Luis Garcia. IEEE M&N 2022. -->

## Online Methods
* [Web-FTP: A Feature Transferring-Based Pre-Trained Model for Web Attack Detection](https://ieeexplore.ieee.org/abstract/document/10854996/). Zhenyu Guo. `TKDE 2025`.
* [Less is More: Simplifying Network Traffic Classification Leveraging RFCs](https://dl.acm.org/doi/abs/10.1145/3701716.3715492). Nimesha Wickramasinghe. `WWW 2025`.
* [Leo: Online ML-based Traffic Classification at Multi-Terabit Line Rate](https://www.usenix.org/conference/nsdi24/presentation/jafri). Syed Usman Jafri. `NSDI 2024`. [[code]](https://github.com/Purdue-ISL/Leo)
* [Brain-on-Switch: Towards Advanced Intelligent Network Data Plane via NN-Driven Traffic Analysis at Line-Speed](https://www.usenix.org/conference/nsdi24/presentation/yan). Jinzhu Yan. `NSDI 2024`. [[code]](https://github.com/InspiringGroup-Lab/Brain-on-Switch)
* [LINC: Enabling Low-Resource In-network Classification and Incremental Model Update](https://smartinternet.group/wp-content/uploads/2024/09/paper-yhl-linc-icnp.pdf). Haolin Yan. `ICNP 2024`. [[code]](https://github.com/haolinyan/LINC)
* [IIsy: Hybrid In-Network Classification Using Programmable Switches](https://ieeexplore.ieee.org/document/10439067). Changgang Zheng. `ToN 2024`. [[code]](https://github.com/In-Network-Machine-Learning/IIsy)
* [Recursive Multi-Tree Construction With Efficient Rule Sifting for Packet Classification on FPGA](https://ieeexplore.ieee.org/document/10315073). Yao Xin. `ToN 2024`. [[code]](https://github.com/wenjunpaper/KickTree)
* [NetVigil: Robust and Low-Cost Anomaly Detection for East-West Data Center Security](https://www.usenix.org/system/files/nsdi24-hsieh.pdf). Kevin Hsieh. `NSDI 2024`. [[code]](https://github.com/microsoft/Yatesbury)
* [RIDS: Towards Advanced IDS via RNN Model and Programmable Switches Co-Designed Approaches](https://ieeexplore.ieee.org/document/10621290). Ziming Zhao. `INFOCOM 2024`. [[code]](https://github.com/Secbrain/RIDS/)
* [Genos: General In-Network Unsupervised Intrusion Detection by Rule Extraction](https://arxiv.org/abs/2403.19248). Ruoyu Li. `INFOCOM 2024`.
* [HorusEye: A Realtime IoT Malicious Traffic Detection Framework using Programmable Switches](https://www.usenix.org/conference/usenixsecurity23/presentation/dong-yutao). Yutao Dong. `USENIX Security 2023`. [[code]](https://github.com/vicTorKd/HorusEye)
* [Detecting Unknown Encrypted Malicious Traffic in Real Time via Flow Interaction Graph Analysis](https://www.ndss-symposium.org/ndss-paper/detecting-unknown-encrypted-malicious-traffic-in-real-time-via-flow-interaction-graph-analysis/). Chuanpu Fu. `NDSS 2023`. [[code]](https://github.com/fuchuanpu/HyperVision)
* [Kitsune: An Ensemble of Autoencoders for Online Network Intrusion Detection](https://www.ndss-symposium.org/wp-content/uploads/2018/02/ndss2018_03A-3_Mirsky_paper.pdf). Yisroel Mirsky. `NDSS 2018`. [[code]](https://github.com/ymirsky/Kitsune-py)

# Measurement
* Domain Name System
    * [A Worldwide View on the Reachability of Encrypted DNS Services](https://dl.acm.org/doi/abs/10.1145/3589334.3645539). Ruixuan Li. `WWW 2024`.
    * [Investigating Deployment Issues of DNS Root Server Instances from a China-wide View](https://ieeexplore.ieee.org/abstract/document/10460172/keywords#keywords). Fenglu Zhang. `IEEE Transactions on Dependable and Secure Computing (TDSC) 2024`.
* Privacy and Security
    * [Enhanced Dynamics of IP Allocation: Fine-Grained IP Geolocation via Temporal-Spatial Correlation](). Yiyang Huang. `IEEE Transactions on Networking (ToN) 2025`.
    * [Mapping the unseen: Robust IP geolocation through the lens of uncertainty quantification](https://www.sciencedirect.com/science/article/abs/pii/S138912862500372X). Xueting Liu. `Computer Networks 2025`.
    * [Privacy protection of China’s top websites: A Multi-layer privacy measurement via network behaviours and privacy policies](https://www.sciencedirect.com/science/article/abs/pii/S0167404822000050). Xinjie Lin. `ComSec 2022`.
    * [Towards IP-based Geolocation via Fine-grained and Stable Webcam Landmarks](https://dl.acm.org/doi/10.1145/3366423.3380216). Zhihao Wang. `WWW 2020`.
    * [Server-Side Traffic Analysis Reveals Mobile Location Information over the Internet](https://ieeexplore.ieee.org/document/8413110). Keen Sung. `IEEE Transactions on Mobile Computing 2018`.
* IPv6
    * [IPv6 Prefix Target Generation through Pattern and Distribution Learning using Vision-Transformer and Guided-Diffusion](https://ieeexplore.ieee.org/document/11044676). Yaochen Ren. `INFOCOM 2025`.
    * [6GAN: IPv6 Multi-Pattern Target Generation via Generative Adversarial Nets with Reinforcement Learning](https://ieeexplore.ieee.org/document/9488912). Tianyu Cui. `INFOCOM 2021`. [[code]](https://github.com/CuiTianyu961030/6GAN)
    * [SiamHAN: IPv6 Address Correlation Attacks on TLS Encrypted Traffic via Siamese Heterogeneous Graph Attention Network](https://www.usenix.org/conference/usenixsecurity21/presentation/cui). Tianyu Cui. `USENIX Security 2021`. [[code]](https://github.com/CuiTianyu961030/SiamHAN)
    * [6VecLM: Language Modeling in Vector Space for IPv6 Target Generation](https://link.springer.com/chapter/10.1007%2F978-3-030-67667-4_12). Tianyu Cui. `ECML/PKDD 2020`. [[code]](https://github.com/CuiTianyu961030/6VecLM)
* Quality of Service
    * [Network Traffic Statistical Upper Limit Prediction From Flow Features for Traffic Fluctuations](https://xplorestaging.ieee.org/document/11143543). Erina Takeshita. `ToN 2025`.

<!--
# Ethereum
* [A Flexible Sharding Blockchain Protocol Based on Cross-Shard Byzantine Fault Tolerance](https://ieeexplore.ieee.org/abstract/document/10100734). Yizhong Liu. TIFS 2023.
* [Secure and Scalable Cross-Domain Data Sharing in Zero-Trust Cloud-Edge-End Environment Based on Sharding Blockchain](https://ieeexplore.ieee.org/abstract/document/10246351). Yizhong Liu. TDSC 2023.
* [TGC: Transaction Graph Contrast Network for Ethereum Phishing Scam Detection](https://dl.acm.org/doi/abs/10.1145/3627106.3627109). Sijia Li. ACSAC 2023.
* [TTAGN: Temporal transaction aggregation graph network for ethereum phishing scams detection](https://dl.acm.org/doi/abs/10.1145/3485447.3512226). Sijia Li. WWW 2022.
-->

# Research Groups
<details>
<summary>
    Chinese Academy of Sciences, University of Chinese Academy of Sciences/China
</summary>

* [Gang Xiong](https://people.ucas.ac.cn/~xionggang) (Institute of Information Engineering)
* [Kai Chen](https://people.ucas.ac.cn/~kaichen) (Institute of Information Engineering)
* [Qixu Liu](https://people.ucas.ac.cn/~liuqixu) (Institute of Information Engineering)
* [Guozhu Meng](https://people.ucas.ac.cn/~gzmeng) (Institute of Information Engineering)
* [Qingyun Liu](https://people.ucas.ac.cn/~0027674) (Institute of Information Engineering)
* [Zhigang Lu](https://people.ucas.ac.cn/~luzhigang) (Institute of Information Engineering)
* [Xiaodong Li](https://people.ucas.edu.cn/~LEE) (Institute of Computing Technology)
* [Zhenyu Li](http://www.ict.ac.cn/sourcedb_2018_ict_cas/cn/jssrck/201111/t20111114_3395505.html) (Institute of Computing Technology)
* [Yujun Zhang](https://people.ucas.ac.cn/~yujun) (Institute of Computing Technology)
* [Yuqing Zhang](https://people.ucas.ac.cn/~zhangyuqing) (School of Computer Science and Technology)
</details>

<details>
<summary>
    Tsinghua University/China
</summary>

* [Ke Xu](http://www.thucsnet.org/xuke.html)
* [Jiahai Yang](https://nmgroup.tsinghua.edu.cn/yjh/)
* [Haixin Duan](http://netsec.ccert.edu.cn/people/duanhx/)
* [Jianjun Chen](https://www.jianjunchen.com/)
* [Dan Li](https://www.cs.tsinghua.edu.cn/info/1126/3948.htm)
* [Yong Cui](https://www.cs.tsinghua.edu.cn/info/1126/3589.htm)
* [Mingwei Xu](https://www.cs.tsinghua.edu.cn/info/1126/3580.htm)
* [Xia Yin](https://www.cs.tsinghua.edu.cn/info/1126/3578.htm)
* [Qi Li](https://www.insc.tsinghua.edu.cn/info/1157/2851.htm)
* [Dan Pei](https://www.cs.tsinghua.edu.cn/info/1127/3597.htm)
* [Zhiliang Wang](https://www.cs.tsinghua.edu.cn/info/1127/3593.htm)
* [Chao Zhang](https://netsec.ccert.edu.cn/chs/people/chaoz/)
</details>

<details>
<summary>
Zhejiang University/China
</summary>

* [Shouling Ji](https://person.zju.edu.cn/sji#0)
* [Wenyuan Xu](https://person.zju.edu.cn/wyxu#0)
* [Meng Luo](https://person.zju.edu.cn/mengluo#0)
* [Kui Ren](https://person.zju.edu.cn/kuiren)
* [Fan Zhang](https://person.zju.edu.cn/fanzhang)
</details>

<details>
<summary>
Harbin Institute of Technology/China
</summary>

* [Weizhe (James) Zhang](https://homepage.hit.edu.cn/wzzhang)
* [Xiangzhan Yu](https://homepage.hit.edu.cn/yuxiangzhan)
* [Hui (Sophia) He](https://homepage.hit.edu.cn/huihe)
* [Junbao Li](https://homepage.hit.edu.cn/lijunbao)
* [Zhaoxin Zhang](https://homepage.hit.edu.cn/zhangzhaoxin)
</details>

<details>
    <summary>
        Beijing University of Posts and Telecommunications/China
    </summary>

* [Shize Guo](https://scss.bupt.edu.cn/info/1063/5386.htm)
* [Dongbin Wang](https://scss.bupt.edu.cn/info/1249/5098.htm)
* [Zhongliang Yang](https://scss.bupt.edu.cn/info/1247/5070.htm)
</details>

<details>
<summary>
    Beijing Institute of Technology/China
</summary>    
    
* [Changzhen Hu](https://cst.bit.edu.cn/szdw/jsml/bssds/ca94335a79114dbe9ae967e53ca86bec.htm)
* [Liehuang Zhu](https://cs.bit.edu.cn/szdw/jsml/wlkjaqxy/zlh/index.htm)
* [Meng Shen](https://cst.bit.edu.cn/szdw/jsml/bssds/86728e84066248b0b13bdf04f685817f.htm)
* [Xuhui Ding](https://cst.bit.edu.cn/szdw/jsml/bssds/711aba6ea79b41618a2f2fac616652a9.htm)
</details>

<details>
<summary>
    Beihang University/China
</summary>    
    
* [Jian Mao](https://shi.buaa.edu.cn/maojian/zh_CN/index.htm)
* [Sheng Hong](http://shi.buaa.edu.cn/hongsheng/zh_CN/index.htm)
* [Ying Gao](https://shi.buaa.edu.cn/gaoying/zh_CN/index.htm)
</details>
    
<details>
<summary>
Xi'an Jiaotong University/China
</summary>
    
* [Xiaohong Guan](https://www.xjtu.edu.cn/jsnr.jsp?wbtreeid=1632&wbwbxjtuteacherid=502)
* [Chao Shen](https://gr.xjtu.edu.cn/web/cshen)
</details>
    
<details>
<summary>
Shanghai Jiao Tong University/China
</summary>
    
* [Guoxing Chen](https://donnod.github.io/)
* [Haojin Zhu](https://nsec.sjtu.edu.cn/~hjzhu/)
</details>

<details>
<summary>
Fudan University/China
</summary>
    
* [Min Yang](https://cs.fudan.edu.cn/3e/d7/c25921a278231/page.htm)
* [Mi Zhang](https://mi-zhang-fdu.github.io/) (Whitzard AI Team)
* [Yuan Zhang](https://yuanxzhang.github.io/)
</details>

<details>
<summary>
    Others
</summary>

* [Guang Cheng](https://cyber.seu.edu.cn/cg1/list.htm) (Southeast University/China)
* [Fengwei Zhang](https://fengweiz.github.io/) (Southern University of Science and Technology/China)
* [Qian Wang](http://nisplab.whu.edu.cn/people.html) (Wuhan University/China)
* [Shuguang Cui](https://sse.cuhk.edu.cn/en/faculty/cuishuguang) (The Chinese University of Hong Kong/China)
* [Feng Li](https://funglee.github.io/) (Shandong University/China)
* [Zhihong Tian](https://scholar.google.com/citations?user=oy9xqxcAAAAJ&hl=en) (Guangzhou University)
</details>
  
<details>
<summary>
Overseas
</summary>
    
* [Xuemin (Sherman) Shen](https://uwaterloo.ca/scholar/sshen) (University of Waterloo/Canada)
* [Xiaofeng Wang](https://homes.luddy.indiana.edu/xw7/) (Indiana University Bloomington/United States)
* [Tao Wang](https://www.cs.sfu.ca/~taowang/) (Simon Fraser University/Canada)
* [Ivan Martinovic](https://www.cs.ox.ac.uk/people/ivan.martinovic/) (University of Oxford/United Kingdom)
* [Amir Houmansadr](https://people.cs.umass.edu/~amir/) (University of Massachusetts Amherst/United States)
* [Giuseppe Aceto](http://wpage.unina.it/giuseppe.aceto/) (University Federico II of Naples/Italy)
* [Antonio Pescapè](http://wpage.unina.it/pescape/) (University Federico II of Naples/Italy)
* [Verdoliva Luisa](https://www.grip.unina.it/members/verdoliva) (University Federico II of Naples/Italy)
* [Thorsten Holz](https://cispa.de/en/research/groups/holz) (CISPA Helmholtz Center for Information Security/Germany)
* [Mohammad Saidur Rahman](https://www.rahmanmsaidur.com/) (University of Texas at El Paso/United States)
* [Yue Zhang](https://yue.zyueinfosec.com/) (Drexel University/United States)
* [Xinyu Xing](http://xinyuxing.org/) (Northwestern University/United States)
* [Yang Liu](https://personal.ntu.edu.sg/yangliu/) (Nanyang Technological University/Singapore)
* [Alessandro Finamore](https://afinamore.io/) (Huawei Technologies/France)
* [Thijs van Ede](https://thijsvane.de/) (University of Twente/Netherlands)
* [Idilio Drago](https://www.cs.unito.it/do/docenti.pl/Alias?idilio.drago#tab-profilo) (University of Turin/Italy)
* [Arash Shaghaghi](https://research.unsw.edu.au/people/dr-arash-shaghaghi) (University of New South Wales/Australia)
</details>

<!-- Wait dor updating
PRL (Privacy Research Lab)	Princeton University	网络隐私、加密通信、流量特征分析	🟢 活跃
Computer Security and Industrial Cryptography (COSIC)	KU Leuven (比利时)	加密协议、网络匿名性、安全通信	🟢 活跃
Network and Distributed Systems Security (NDSS Lab)	UC Irvine	加密协议、匿名通信分析	🟢 活跃
Information Security Group (ISG)	Royal Holloway, University of London	流量分析、TLS/QUIC研究	🟢 活跃
SecLab	Northeastern University	加密通信、网络测量、反审查	🟢 活跃
Security and Privacy Engineering Lab (SPRITE)	Georgia Tech	加密流量、IoT安全、数据保护	🟢 活跃
CISPA Helmholtz Center	德国	加密通信协议分析、网络匿名性
-->

# Blogs
## Network Traffic Knowledge
* [Icoding_F2014](https://blog.csdn.net/jmh1996)
* [Malware-Traffic-Analysis](https://www.malware-traffic-analysis.net/)
* [Awesome-NTA](https://github.com/wangtz19/Awesome-NTA)

<!--
## Network Traffic Analysis Tool Manual
https://dilidonglong.com/2019/04/26/tshark%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95/
-->

# Tool Libraries and Frameworks
* [PacketScope](https://github.com/Internet-Architecture-and-Security/PacketScope)
* [flowcontainer](https://github.com/jmhIcoding/flowcontainer)
* [scapy](https://scapy.net/)
* [wireshark](https://www.wireshark.org/)
* [Tshark](https://www.wireshark.org/docs/man-pages/tshark.html)
* [pyshark](https://kiminewt.github.io/pyshark/)
* [Cisco Talos](https://talosintelligence.com/software)
* [Joy](https://github.com/cisco/joy)
* [Proxifier](https://www.proxifier.com/)
* [traffic_classification_utils](https://github.com/jmhIcoding/traffic_classification_utils)
* [Website-Fingerprinting-Library (WFlib)](https://github.com/Xinhao-Deng/Website-Fingerprinting-Library)
* [NTC-Enigma](https://github.com/nime-sha256/ntc-enigma)
* [CICFlowMeter](https://github.com/ahlashkari/CICFlowMeter)

# News and Updates
**Version 2.0**
> March 22, 2025 
1. Welcome to the New Contributors from UCAS, BIT, SEU, GZHU!
2. The content is presented with a clearer structure and style.
3. Fixed some errors.

**Version 1.0**
> April 15, 2022 
1. Welcome to the Ph.Ds from IIE,CAS.

# Contributors 🌟

Thanks goes to these wonderful people!

<table>
  <tr>
    <td align="center"><a href="https://github.com/linwhitehat"><img src="https://avatars3.githubusercontent.com/u/20349381?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Xinjie Lin</b></sub></a><br /><a href="#ideas-XinjieLin" title="Ideas, Planning, & Feedback">🎯</a> <a href="https://github.com/linwhitehat/ETA-Resource/commits?author=linwhitehat" title="Documentation">📝</a> <a href="#maintenance-XinjieLin" title="Maintenance">📔</a></td>
    <td align="center"><a href="https://github.com/CuiTianyu961030"><img src="https://avatars.githubusercontent.com/u/43595189?v=4" width="100px;" alt=""/><br /><sub><b>Tianyu Cui</b></sub></a><br /><a href="#ideas-TianyuCui" title="Ideas, Planning, & Feedback">🎯</a> </td>
    <td align="center"><a href="https://github.com/jmhIcoding"><img src="https://avatars.githubusercontent.com/u/19209689?v=4" width="100px;" alt=""/><br /><sub><b>Minghao Jiang</b></sub></a><br /><a href="#ideas-MinghaoJiang" title="Ideas, Planning, & Feedback">🎯</a> </td>
    <td align="center"><a href="https://github.com/GuanZH95"><img src="https://avatars.githubusercontent.com/u/30852909?v=4" width="100px;" alt=""/><br /><sub><b>Zhong Guan</b></sub></a><br /><a href="#ideas-ZhongGuan" title="Ideas, Planning, & Feedback">🎯</a> <a href="https://github.com/linwhitehat/ETA-Resource/commits?author=GuanZH95" title="Documentation">📝</a></td>
    <td align="center"><a href="https://github.com/wayneowen7"><img src="https://avatars.githubusercontent.com/u/29433723?v=4" width="100px;" alt=""/><br /><sub><b>Wei Cai</b></sub></a><br /><a href="#ideas-WeiCai" title="Ideas, Planning, & Feedback">🎯</a> </td>
    <td align="center"><a href="https://github.com/XiyuanZhang97"><img src="https://avatars.githubusercontent.com/u/205738959?v=4" width="100px;" alt=""/><br /><sub><b>Xiyuan Zhang</b></sub></a><br /><a href="#ideas-XiyuanZhang" title="Ideas, Planning, & Feedback">🎯</a> </td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/yyyjn"><img src="https://avatars.githubusercontent.com/u/32609644?s=400&v=4" width="100px;" alt=""/><br /><sub><b>Junnan Yin</b></sub></a><br /><a href="#ideas-JunnanYin" title="Ideas, Planning, & Feedback">🎯</a> <a href="https://github.com/linwhitehat/ETA-Resource/commits?author=yyyjn" title="Documentation">📝</a></td>
    <td align="center"><a href="https://github.com/TaRiK-Haob"><img src="https://avatars.githubusercontent.com/u/83114553?v=4" width="100px;" alt=""/><br /><sub><b>TaRiK-Haob</b></sub></a><br /><a href="https://github.com/linwhitehat/ETA-Resource/commits?author=TaRiK-Haob" title="Documentation">📝</a></td>
    <td align="center"><a href="https://github.com/weiyuhao2021"><img src="https://avatars.githubusercontent.com/u/89506254?v=4" width="100px;" alt=""/><br /><sub><b>Yuhao Wei</b></sub></a><br /><a href="https://github.com/linwhitehat/ETA-Resource/commits?author=YuhaoWei" title="Documentation">📝</a></td>
    <td align="center"><a href="https://github.com/Frederick666666"><img src="https://avatars.githubusercontent.com/u/75159200?v=4" width="100px;" alt=""/><br /><sub><b>Wenqi Dong</b></sub></a><br /><a href="https://github.com/linwhitehat/ETA-Resource/commits?author=WenqiDong" title="Documentation">📝</a></td>
    <td align="center"><a href="https://github.com/iiehyy"><img src="https://avatars.githubusercontent.com/u/186914194?v=4" width="100px;" alt=""/><br /><sub><b>Yiyang Huang</b></sub></a><br /><a href="https://github.com/linwhitehat/ETA-Resource/commits?author=YiyangHuang" title="Documentation">📝</a></td>
    <td align="center"><a href="https://github.com/xingyue-Wangh"><img src="https://avatars.githubusercontent.com/u/85674037?v=4" width="100px;" alt=""/><br /><sub><b>xingyue-Wangh</b></sub></a><br /><a href="https://github.com/linwhitehat/ETA-Resource/commits?author=xingyue-Wangh" title="Documentation">📝</a></td>
  </tr>
  <tr>
  <td align="center"><a href="https://github.com/nime-sha256"><img src="https://avatars.githubusercontent.com/u/27483081?v=4" width="100px;" alt=""/><br /><sub><b>Nimesha Wickramasinghe</b></sub></a><br /><a href="#ideas-nime-sha256" title="Ideas, Planning, & Feedback">🎯</a> <a href="https://github.com/linwhitehat/ETA-Resource/commits?author=nime-sha256" title="Documentation">📝</a></td>
  </tr>
</table>
