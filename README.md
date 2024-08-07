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
- [Network Traffic Classification](#network-traffic-classification)
- [Measurement](#measurement)
- [Ethereum](#ethereum)
- [Teams](#teams)
- [Blogs](#blogs)
- [Libraries and Frameworks](#tool-libraries-and-frameworks)

# About
This is a current list of resources related to the research and development of encrypted traffic analysis. We comb the field for relevant representative work and related resources, and pay more attention to typical studies and research teams.

# Datasets
* [Canadian Institute for Cybersecurity Datasets](https://www.unb.ca/cic/datasets/) (DNS, IDS, DoS, Darknet, Tor, VPN, Botnet, Malware)
* [Cross-Platform](https://recon.meddle.mobi/cross-market.html) (iOS and Android Apps)
* [Malware Capture Facility Project](https://www.stratosphereips.org/datasets-overview) (Malware)
* [CSTNET-TLS 1.3](https://drive.google.com/drive/folders/1JSsYmevkxQFanoKOi_i1ooA6pH3s9sDr?usp=sharing) (TLS 1.3 services)
* [Network-based Intrusion Detection](https://www.sciencedirect.com/science/article/pii/S016740481930118X) (AWID, Botnet, CIC DoS, CICIDS, CIDDS, CTU, DARPA, ISCX, IRSC)
* [MobileTraffic](https://github.com/Abby-ZS/NUDT_MobileTraffic) (300+ Mobile Apps)
* [Itc-Net-Blend-60](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4661706) (Android applications in Diverse Environments)
* [Network-Flow-of-QUIC](https://drive.google.com/drive/folders/1cwHhzvaQbi-ap8yfrj2vHyPmUTQhaYOj) (QUIC services)

# Survey
* [Deep Learning for Encrypted Traffic Classification: An Overview](https://ieeexplore.ieee.org/document/8713803/). Shahbaz Rezaei. IEEE Communications Magazine 2019.
* [Towards the Deployment of Machine Learning Solutions in Network Traffic Classification: A Systematic Survey](https://ieeexplore.ieee.org/document/8543584). Fannia Pacheco. IEEE Communications Surveys & Tutorials 2019.
* [Deep Learning in Mobile and Wireless Networking: A Survey](https://ieeexplore.ieee.org/document/8666641). Chaoyun Zhang. IEEE Communications Surveys & Tutorials 2019.

# Network Traffic Classification

## Traditional Target (Web, App, Malware, Gambling)
* [Point Cloud Analysis for ML-Based Malicious Traffic Detection: Reducing Majorities of False Positive Alarms](https://dl.acm.org/doi/10.1145/3576915.3616631). Chuanpu Fu. CCS 2023.
* [Detecting Unknown Encrypted Malicious Traffic in Real Time via Flow Interaction Graph Analysis](https://www.ndss-symposium.org/wp-content/uploads/2023/02/ndss2023_s80_paper.pdf). Chuanpu Fu. NDSS 2023.
* [Gambling Domain Name Recognition via Certificate and Textual Analysis](https://academic.oup.com/comjnl/article/66/8/1829/6570684). GuoYing Sun. The Computer Journal 2023.
* [Analyzing Ground-Truth Data of Mobile Gambling Scams](https://ieeexplore.ieee.org/abstract/document/9833665). Geng Hong. Symposium on Security and Privacy(S&P) 2022.
* [Classifying encrypted traffic using adaptive fingerprints with multi-level attributes](https://link.springer.com/article/10.1007%2Fs11280-021-00940-0). Chang Liu. WWW Journal 2021.
* [CETAnalytics: Comprehensive effective traffic information analytics for encrypted traffic classification](https://www.sciencedirect.com/science/article/pii/S1389128619309466) (Generalization). Cong Dong. Computer Networks 2020.
* [FlowPrint: Semi-Supervised Mobile-App Fingerprinting on Encrypted Network Traffic](https://www.ndss-symposium.org/wp-content/uploads/2020/02/24412.pdf). van Ede, Thijs. NDSS 2020. [[code]](https://github.com/Thijsvanede/FlowPrint)
* [FS-Net: A Flow Sequence Network For Encrypted Traffic Classification](https://ieeexplore.ieee.org/document/8737507). Chang Liu. INFOCOM 2019. [[code]](https://github.com/WSPTTH/FS-Net)
* [MaMPF: Encrypted Traffic Classification Based on Multi-Attribute Markov Probability Fingerprints](https://ieeexplore.ieee.org/abstract/document/8624124).  Chang Liu. IWQoS 2018. [[code]](https://github.com/WSPTTH/MaMPF)
* [AppScanner: Automatic Fingerprinting of Smartphone Apps from Encrypted Network Traffic](https://ieeexplore.ieee.org/abstract/document/7467370). Vincent F. Taylor. EuroS&P 2016. [[code]](https://github.com/vftaylor/appscanner)

## Anonymous and VPN
* [Real-Time Website Fingerprinting Defense via Traffic Cluster Anonymization](). Meng Shen. Symposium on Security and Privacy(S&P) 2024.
* [HSDirSniper: A New Attack Exploiting Vulnerabilities in Tor's Hidden Service Directories](https://dl.acm.org/doi/10.1145/3589334.3645591). Qingfeng Zhang. WWW 2024.
* [VPNSniffer: Identifying VPN Servers Through Graph-Represented Behaviors](https://dl.acm.org/doi/10.1145/3589334.3645552). Chenxu Wang. WWW 2024.
* [Subverting Website Fingerprinting Defenses with Robust Traffic Representation](https://www.usenix.org/conference/usenixsecurity23/presentation/shen-meng). Meng Shen. USENIX 2023.
* [Transformer-based Model for Multi-tab Website Fingerprinting Attack](https://dl.acm.org/doi/abs/10.1145/3576915.3623107). Zhaoxin Jin. CCS 2023.
* [Online Website Fingerprinting: Evaluating Website Fingerprinting Attacks on Tor in the Real World](https://www.usenix.org/conference/usenixsecurity22/presentation/cherubin). Giovanni Cherubin. Usenix Security 2022.
* [BAPM: Block Attention Profiling Model for Multi-tab Website Fingerprinting Attacks on Tor](https://dl.acm.org/doi/10.1145/3485832.3485891). Zhong Guan. ACSAC 2021.
* [Deep Fingerprinting: Undermining Website Fingerprinting Defenses with Deep Learning](https://dl.acm.org/doi/abs/10.1145/3243734.3243768). Payap Sirinam. CCS 2018. [[code]](https://github.com/deep-fingerprinting/df)

## ETA with Pre-training/LLMs (Generalization)
* [CETP: A Novel Semi-Supervised Framework Based on Contrastive Pre-Training for Imbalanced Encrypted Traffic Classification](https://www.sciencedirect.com/science/article/abs/pii/S0167404824001949). Xinjie Lin. Computers & Security 2024.
* [Listen to Minority: Encrypted Traffic Classification for Class Imbalance with Contrastive Pre-Training](https://ieeexplore.ieee.org/abstract/document/10287449). Xiang Li. SECON 2023.
* [Yet Another Traffic Classifier: A Masked Autoencoder Based Traffic Transformer with Multi-Level Flow Representation](https://ojs.aaai.org/index.php/AAAI/article/view/25674). Ruijie Zhao. AAAI 2023.
* [ET-BERT: A Contextualized Datagram Representation with Pre-training Transformers for Encrypted Traffic Classification](https://dl.acm.org/doi/abs/10.1145/3485447.3512217). Xinjie Lin. WWW 2022. [[code]](https://github.com/linwhitehat/et-bert) [[Reproduce]](https://gitee.com/xxdxxdxxd/et-bert/blob/master/README.md)

## ETA for Stable/Robust (Out-of-Distribution, Few-shot, Zero-shot)
* [Rosetta: Enabling Robust TLS Encrypted Traffic Classification in Diverse Network Environments with TCP-Aware Traffic Augmentation](https://www.usenix.org/conference/usenixsecurity23/presentation/xie). Renjie Xie. USENIX 2023.
* [Zero-relabelling mobile-app identification over drifted encrypted network traffic](https://doi.org/10.1016/j.comnet.2023.109728). Minghao Jiang. Computer Networks 2023.
* [Anomaly Detection in the Open World: Normality Shift Detection, Explanation, and Adaptation](https://www.ndss-symposium.org/ndss-paper/anomaly-detection-in-the-open-world-normality-shift-detection-explanation-and-adaptation/). Dongqi Han. NDSS 2023. [[code]](https://github.com/dongtsi/OWAD)
* [Accurate mobile-app fingerprinting using flow-level relationship with graph neural networks](https://www.sciencedirect.com/science/article/pii/S1389128622003577). Minghao Jiang. Computer Networks 2022.
* [Triplet Fingerprinting: More Practical and Portable Website Fingerprinting with N-shot Learning](https://dl.acm.org/doi/abs/10.1145/3319535.3354217). Payap Sirinam. CCS 2019. [[code]](https://github.com/triplet-fingerprinting/tf) (N-shot Learning)

## IoT
* [HorusEye: A Realtime IoT Malicious Traffic Detection Framework using Programmable Switches](https://www.usenix.org/conference/usenixsecurity23/presentation/dong-yutao). Yutao Dong. USENIX 2023.

## Vedio (Streaming Media)
* [Traffic spills the beans: A robust video identification attack against YouTube](https://www.sciencedirect.com/science/article/abs/pii/S0167404823005333). Xiyuan Zhang. Computers & Security 2024.
* [Walls Have Ears: Traffic-based Side-channel Attack in Video Streaming](https://ieeexplore.ieee.org/abstract/document/8486211). Jiaxi Gu. IEEE INFOCOM 2018.

# Measurement
* [6GAN: IPv6 Multi-Pattern Target Generation via Generative Adversarial Nets with Reinforcement Learning](https://ieeexplore.ieee.org/document/9488912). Tianyu Cui. INFOCOM 2021. [[code]](https://github.com/CuiTianyu961030/6GAN)
* [SiamHAN: IPv6 Address Correlation Attacks on TLS Encrypted Traffic via Siamese Heterogeneous Graph Attention Network](https://www.usenix.org/conference/usenixsecurity21/presentation/cui). Tianyu Cui. USENIX 2021. [[code]](https://github.com/CuiTianyu961030/SiamHAN)
* [6VecLM: Language Modeling in Vector Space for IPv6 Target Generation](https://link.springer.com/chapter/10.1007%2F978-3-030-67667-4_12). Tianyu Cui. ECML/PKDD 2020. [[code]](https://github.com/CuiTianyu961030/6VecLM)

# Ethereum
* [A Flexible Sharding Blockchain Protocol Based on Cross-Shard Byzantine Fault Tolerance](https://ieeexplore.ieee.org/abstract/document/10100734). Yizhong Liu. TIFS 2023.
* [Secure and Scalable Cross-Domain Data Sharing in Zero-Trust Cloud-Edge-End Environment Based on Sharding Blockchain](https://ieeexplore.ieee.org/abstract/document/10246351). Yizhong Liu. TDSC 2023.
* [TGC: Transaction Graph Contrast Network for Ethereum Phishing Scam Detection](https://dl.acm.org/doi/abs/10.1145/3627106.3627109). Sijia Li. ACSAC 2023.
* [TTAGN: Temporal transaction aggregation graph network for ethereum phishing scams detection](https://dl.acm.org/doi/abs/10.1145/3485447.3512226). Sijia Li. WWW 2022.

# Teams
* Tsinghua University/China
    * [Ke Xu](http://www.thucsnet.org/xuke.html)
    * [Jiahai Yang](https://nmgroup.tsinghua.edu.cn/yjh/)
    * [Haixin Duan](http://netsec.ccert.edu.cn/people/duanhx/)
* Chinese Academy of Sciences/China
    * [Gang Xiong](https://people.ucas.ac.cn/~xionggang) (Institute of Information Engineering)
    * [Zhenyu Li](http://www.ict.ac.cn/sourcedb_2018_ict_cas/cn/jssrck/201111/t20111114_3395505.html) (Institute of Computing Technology)
* Beijing Institute of Technology/China
    * [Liehuang Zhu](https://cs.bit.edu.cn/szdw/jsml/wlkjaqxy/zlh/index.htm)
    * [Meng Shen](https://cst.bit.edu.cn/szdw/jsml/bssds/86728e84066248b0b13bdf04f685817f.htm)
* [Binxing Fang](https://www.gzhu.edu.cn/info/1105/3650.htm) (Guangzhou University/China)
* [Xiaohong Guan](https://www.xjtu.edu.cn/jsnr.jsp?wbtreeid=1632&wbwbxjtuteacherid=502) (Xi'an Jiaotong University/China)
* [Guang Cheng](https://cyber.seu.edu.cn/cg1/list.htm) (Southeast University/China)
* Overseas Teams
    * [Tao Wang](https://www.cs.sfu.ca/~taowang/) (Simon Fraser University/Canada)
    * [Xiaofeng Wang](https://homes.luddy.indiana.edu/xw7/) (Indiana University Bloomington/United States)
    * [Ivan Martinovic](https://www.cs.ox.ac.uk/people/ivan.martinovic/) (University of Oxford/United Kingdom)
    * [Amir Houmansadr](https://people.cs.umass.edu/~amir/) (University of Massachusetts Amherst/United States)

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
