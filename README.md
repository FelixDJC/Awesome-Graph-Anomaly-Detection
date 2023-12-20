[stars-img]: https://img.shields.io/github/stars/FelixDJC/Awesome-Graph-Anomaly-Detection?color=yellow
[stars-url]: https://github.com/FelixDJC/Awesome-Graph-Anomaly-Detection/stargazers
[fork-img]: https://img.shields.io/github/forks/FelixDJC/Awesome-Graph-Anomaly-Detection?color=lightblue&label=fork
[fork-url]: https://github.com/FelixDJC/Awesome-Graph-Anomaly-Detection/network/members

# Awesome Graph Anomaly Detection 
Collections for state-of-the-art (SOTA), novel awesome graph anomaly detecion methods (papers, codes and datasets)

We are looking forward for other participants to share their papers and codes. If interested, please contanct <jingcan_duan@163.com> or jinhu@nudt.edu.cn.

[![GitHub stars][stars-img]][stars-url]
[![GitHub forks][fork-img]][fork-url]


## Table of Contents

- [Surveys](#jump1) 
- [Papers and Codes](#jump2)
  - [Single-View Static Graph](#jump21)
  - [Multi-View Static Graph](#jump22)
  - [Temporal Graph](#jump23)
  - [Others](#jump24)
- [Benchmark Datasets](#jump3)
  - [Injected Datasets](#jump31)
  - [Real-world Anomaly Datasets](#jump32)
- [Other Related Awesome Repository](#jump4)

---

## <span id="jump1">Important Survey and Benchmark Papers</span>
1. TKDE 2021: A Comprehensive Survey on Graph Anomaly Detection with Deep Learning [[Paper]](https://arxiv.org/pdf/2106.07178.pdf)
2. NeurIPS 2022: BOND: Benchmarking Unsupervised Outlier Node Detection on Static Attributed Graphs [[Paper]](https://openreview.net/pdf?id=YXvGXEmtZ5N) [[Code]](https://github.com/pygod-team/pygod)

---

## <span id="jump2">Papers and Codes</span>
### <span id="jump21">Single-View Static Graph</span>
Papers focus on node-level anomaly detection and work on single-view static graph datasets.
#### <span>Traditional Methods</span>
1. SIGMOD 2000: 
LOF: Identifying Density-based Local Outliers [[Paper]](https://dl.acm.org/doi/pdf/10.1145/342009.335388)[[Code]](https://github.com/damjankuznar/pylof)
2. KDD 2007: SCAN: a Structural Clustering Algorithm for Networks [[Paper]](http://web.cs.ucla.edu/~yzsun/classes/2014Spring_CS7280/Papers/Clustering/SCAN.pdf) [[Code]](https://github.com/gombaniro/SCAN-A-Structural-Clustering-Algorithm-for-Networks)
3. SDM 2016: Scalable Anomaly Ranking of Attributed Neighborhoods [[Paper]](https://epubs.siam.org/doi/pdf/10.1137/1.9781611974348.24)[[Code]](https://github.com/phanein/amen)
4. IJCAI 2017: Radar: Residual Analysis for Anomaly Detection in Attributed Networks [[Paper]](https://www.researchgate.net/profile/Jundong-Li/publication/318830338_Radar_Residual_Analysis_for_Anomaly_Detection_in_Attributed_Networks/links/5a1f17c4458515a4c3d478ce/Radar-Residual-Analysis-for-Anomaly-Detection-in-Attributed-Networks.pdf) [[Code]](https://github.com/szumbrunn/radar-java)
5. IJCAI 2018: ANOMALOUS: A Joint Modeling Approach for Anomaly Detection on Attributed Networks [[Paper]](https://www.ijcai.org/Proceedings/2018/0488.pdf) [[Code]](https://github.com/zpeng27/ANOMALOUS)
#### <span>Deep Methods</span>
##### <span>Reconstruction</span>
1. SDM 2019: Deep Anomaly Detection on Attributed Networks [[Paper]](https://www.researchgate.net/profile/Kaize-Ding/publication/332888297_Deep_Anomaly_Detection_on_Attributed_Networks/links/606f78364585150fe993abb6/Deep-Anomaly-Detection-on-Attributed-Networks.pdf) [[Code]](https://github.com/kaize0409/GCN_AnomalyDetection_pytorch)
2. DSAA 2021: ResGCN: Attention-based Deep Residual Modeling for Anomaly Detection on Attributed Networks [[Paper]](https://link.springer.com/content/pdf/10.1007/s10994-021-06044-0.pdf)[[Code]](https://bitbucket.org/paulpei/resgcn)
3. TKDE 2021: Hybrid-order Anomaly Detection on Attributed Networks [[Paper]](https://ieeexplore.ieee.org/abstract/document/9560054/)[[Code]](https://github.com/zirui-yuan/HO-GAT)
4. WSDM 2022: ComGA: Community-Aware Attributed Graph Anomaly Detection [[Paper]](https://dl.acm.org/doi/abs/10.1145/3488560.3498389)[[Code]](https://github.com/XuexiongLuoMQ/ComGA)
##### <span>Reinforcement Learning</span>
1. WSDM 2019: Interactive Anomaly Detection on Attributed Networks [[Paper]](https://dl.acm.org/doi/pdf/10.1145/3289600.3290964)[[Code]](https://github.com/kaize0409/GraphUCB_AnomalyDetection)
2. CIKM 2021: Towards Anomaly-resistant Graph Neural Networks via Reinforcement Learning [[Paper]](https://www.public.asu.edu/~kding9/pdf/CIKM2021_RARE-GNN.pdf)
3. ICDM 2023: Reinforcement Neighborhood Selection for Unsupervised Graph [[Paper]](https://arxiv.org/abs/2312.05526)[[Code]](https://github.com/YuanchenBei/RAND)
##### <span>Generative Adversarial Network</span>
1. IJCAI 2020: Inductive Anomaly Detection on Attributed Networks [[Paper]](http://www.ece.virginia.edu/~jl6qk/pubs/IJCAI2020-1.pdf) 
2. CIKM 2020: Generative Adversarial Attributed Network Anomaly Detection [[Paper]](https://static.aminer.cn/storage/pdf/acm/20/cikm/10.1145/3340531.3412070.pdf)
        
        
        
        
        
        
        
        
##### <span>Filter</span>
1. IJCAI 2022: Can Abnormality be Detected by Graph Neural Networks? [[Paper]](http://yangy.org/works/gnn/IJCAI22_Abnormality.pdf) [[Code]](https://github.com/zjunet/AMNet)
2. ICML 2022: Rethinking Graph Neural Networks for Anomaly Detection [[Paper]](https://arxiv.org/pdf/2205.15508) [[Code]](https://github.com/squareRoot3/Rethinking-Anomaly-Detection)
3. CIKM 2023: SplitGNN: Spectral Graph Neural Network for Fraud Detection against Heterophily [[Paper]](https://dl.acm.org/doi/10.1145/3583780.3615067)[[Code]](https://github.com/Split-GNN/SplitGNN)
##### <span>One-class SVM</span>
1. CIKM 2021: Subtractive Aggregation for Attributed Network Anomaly Detection [[Paper]](https://www4.comp.polyu.edu.hk/~xiaohuang/docs/Shuang_CIKM21.pdf) 
2. NCA 2021: One-Class Graph Neural Networks for Anomaly Detection in Attributed Networks [[Paper]](https://arxiv.org/pdf/2002.09594) [[Code]](https://github.com/WangXuhongCN/OCGNN)
##### <span>Meta Learning</span>
1. WWW 2021: Few-shot Network Anomaly Detection via Cross-network Meta-learning [[Paper]](https://arxiv.org/pdf/2102.11165) [[Code]](https://github.com/kaize0409/Meta-GDN_AnomalyDetection)
##### <span>Contrastive Learning</span>
1. TNNLS 2021: Anomaly Detection on Attributed Networks via Contrastive Self-Supervised Learning [[Paper]](https://arxiv.org/pdf/2103.00113) [[Code]](https://github.com/GRAND-Lab/CoLA)
2. CIKM 2021: ANEMONE: Graph Anomaly Detection with Multi-Scale Contrastive Learning [[Paper]](https://shiruipan.github.io/publication/cikm-21-jin/cikm-21-jin.pdf) [[Code]](https://github.com/GRAND-Lab/ANEMONE)
3. AAAI 2023: Graph Anomaly Detection via Multi-Scale Contrastive Learning Networks with Augmented View [[Paper]](https://arxiv.org/abs/2212.00535) [[Code]](https://github.com/FelixDJC/GRADATE)
4. ACM MM 2023: Normality Learning-based Graph Anomaly Detection via Multi-Scale Contrastive Learning [[Paper]](https://arxiv.org/abs/2309.06034) [[Code]](https://github.com/FelixDJC/NLGAD)
5. ICDM 2023: PREM: A Simple Yet Effective Approach for Node-Level Graph Anomaly Detection [[Paper]](https://arxiv.org/abs/2310.11676)[[Code]](https://github.com/CampanulaBells/PREM-GAD)
##### <span>Hybrid Methods</span>
1. TKDE 2021: Generative and Contrastive Self-Supervised Learning for Graph Anomaly Detection [[Paper]](https://arxiv.org/pdf/2108.09896) [[Code]](https://github.com/KimMeen/SL-GAD)
2. IJCAI 2022: Reconstruction Enhanced Multi-View Contrastive Learning for Anomaly Detection on Attributed Networks [[Paper]](https://arxiv.org/pdf/2108.09896) [[Code]](https://github.com/Zjer12/Sub)
3. TKDE 2023: Counterfactual Graph Learning for Anomaly Detection on Attributed Networks [[Paper]](https://www.researchgate.net/publication/368909540_Counterfactual_Graph_Learning_for_Anomaly_Detection_on_Attributed_Networks)
4. TNNLS 2023: ARISE: Graph Anomaly Detection on Attributed Networks via Substructure Awareness [[Paper]](https://ieeexplore.ieee.org/document/10258476) [[Code]](https://github.com/FelixDJC/ARISE)
##### <span>Other Self-Supervised Learning</span>
1. Arxiv 2021: Hop-count Based Self-supervised Anomaly Detection on Attributed Networks [[Paper]](https://arxiv.org/pdf/2104.07917) [[Code]](https://github.com/TienjinHuang/GraphAnomalyDetection)
##### <span>Attention</span>
1. ICDM 2023: Dynamic Relation-Attentive Graph Neural Networks for Fraud Detection [[Paper]](https://arxiv.org/pdf/2310.04171.pdf)[[Code]](https://github.com/bdi-lab/DRAG)
##### <span>Others</span>
1. AAAI 2022: LUNAR: Unifying Local Outlier Detection Methods via Graph Neural Networks [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/20629/20388) [[Code]](https://github.com/agoodge/LUNAR)
### <span id="jump22">Multi-View Static Graph</span>
Papers focus on node-level anomaly detection and work on multi-view static graph datasets.
##### <span>Reconstruction</span>
1. TKDE 2022: A Deep Multi-View Framework for Anomaly Detection on Attributed Networks [[Paper]](https://ieeexplore.ieee.org/abstract/document/9162509/) 
### <span id="jump23">Temporal Graph</span>
Papers focus on node-level anomaly detection and work on single-view temporal graph datasets.
### <span id="jump24">Others</span>
Papers focus on graph-level anomaly detection and work on single-view static graph datasets.
1. WSDM 2022: Deep Graph-level Anomaly Detection by Glocal Knowledge Distillation [[Paper]](https://arxiv.org/pdf/2112.10063) [[Code]](https://github.com/RongrongMa/GLocalKD)
2. WSDM 2023: GOOD-D: On Unsupervised Graph Out-Of-Distribution Detection [[Paper]](https://arxiv.org/pdf/2211.04208.pdf) [[Code]](https://github.com/yixinliu233/G-OOD-D)

---

## <span id="jump3">Benchmark Datasets</span>
### <span id="jump3">Single-View Static Graph</span>
#### <span id="jump31">Injected Datasets</span>
By way of injection, adding anomalous nodes to datasets that do not have anomalies before. These anomalous nodes consist of feature anomalies and structure anomalies. The total number of anomalies are shown in the 5th column of table.

| **Dataset**     | **Nodes** | **Edges** | **Features** | **Anomalies** | **URL**                              |
|:---------------:|:---------:|:---------:|:--------------:|:-------------:|:----------------------------------:|
| **BlogCatalog** | 5196      | 171743    | 8189           | 300           | [[BlogCatalog]](https://github.com/GRAND-Lab/CoLA/) |
| **Flickr**      | 7575      | 239738    | 12407          | 450           | [[Flickr]](https://github.com/GRAND-Lab/CoLA/) |
| **ACM**         | 16484     | 71980     | 8337           | 600           | [[ACM]](https://github.com/GRAND-Lab/CoLA/) |
| **Cora**        | 2708      | 5429      | 1433           | 150           | [[Cora]](https://github.com/GRAND-Lab/CoLA/) |
| **Citeseer**    | 3327      | 4732      | 3703           | 150           | [[Citeseer]](https://github.com/GRAND-Lab/CoLA/) |
| **Pubmed**      | 19717     | 44338     | 500            | 600           | [[Pubmed]](https://github.com/GRAND-Lab/CoLA/) |


#### <span id="jump32">Real-world Anomaly Datasets</span>
These datasets are born with anomalous nodes.
| **Datasets**    | **Nodes** | **Edges** | **Features** | **Anomalies** | **URL**                                                        |
|:--------------:|:---------:|:---------:|:--------------:|:-------------:|:-------------------------------------------------------------:|
| **Amazon**     | 1418      | 3695      | 21             | 28            | [[Amazon]](https://github.com/Juintin/GraphAnomalyDetection)             |
| **Enron**      | 13533     | 176987    | 20             | 5             | [[Enron]](https://github.com/Juintin/GraphAnomalyDetection)            |
| **YelpChi**    | 45954     | 3846979   | 32             | 6677          | [[YelpChi]](https://github.com/zjunet/AMNet)                              |
| **T-Finance** | 39357     | 21222543  | 10             | 1803          | [[T-Finance]](https://github.com/squareRoot3/Rethinking-Anomaly-Detection)  |
| **T-Social**  | 5781065   | 73105508  | 10             | 174010        | [[T-Social]](https://github.com/squareRoot3/Rethinking-Anomaly-Detection)  |
| **Elliptic**   | 46564     | 73248     | 93             | 4,545         | [[Elliptic]](https://github.com/zjunet/AMNet)                              |




## <span id="jump4">Other Related Awesome Repository</span>
[awesome-multi-view-clustering](https://github.com/wangsiwei2010/awesome-multi-view-clustering)

[Incomplete Multi-view Clustering](https://github.com/Jeaninezpp/Incomplete-multi-view-clustering)

[Awesome Deep Graph Clustering](https://github.com/yueliu1999/Awesome-Deep-Graph-Clustering)

