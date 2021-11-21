将城市AI中已接触过的论文和数据集整理如下：

[toc]

# Traffic

## Datasets

* DiDi chuxing: https://outreach.didichuxing.com/app-vue/dataList

## Contest

### 路况状态时空预测（已结束）

移动互联网时代的到来让所有移动设备的持有者都可以成为道路通行能力的描绘者, 滴滴平台收集了海量的高质量司乘轨迹数据, 可以对实时道路拥堵状况有良好的建模能力。 如果可以基于实时和历史的路况信息, 对未来的路况状态有较精准的预估, 无疑对出行决策, 缓解城市拥堵等场景有至关重要的作用。 然而, 未来的路况预估仍然是十分困难的, 未来路况会受到时间周期, 道路通行能力, 路网上下游拓扑, 导航流量以及道路突然状况等多种因素的影响。此次竞赛诚邀参赛者基于滴滴提供的实时与历史路况状态信息以及道路属性等信息, 精准预估未来某时间段内的路况状态, 助力城市规划与智能出行方案。**根据滴滴提供的道路小段的实时和历史路况状态特征, 道路基本属性以及路网拓扑关系图, 预测未来一段时间内道路小段的路况状态**(即畅通, 缓行和拥堵几类状态)。

* HomePage LINK：https://www.datafountain.cn/competitions/466

* 举办方：中国计算机学会 & 滴滴出行

* 数据链接：https://outreach.didichuxing.com/app-vue/dataList

### Traffic4cast

Building on its success at [NeurIPS 2019](https://www.iarai.ac.at/traffic4cast/2019-competition/conference/), the Traffic4cast competition is going into its second year offering **new challenges and opportunities**. This year’s dataset will be derived from an order of magnitude more data. We are collecting data from multiple cities of different size, geography, culture, and economy. **The core challenge will be to predict short-term large-scale traffic states in all the cities**. Participants can investigate differences and similarities in traffic patterns between the cities, and explore master models trained on multiple cities. The dataset will be augmented by new static and dynamic features, such as street maps properties, points of interest, and air pollution. Bonus challenges invite participants to explore the effects of these additional features.

[Traffic4cast HomePage](https://www.iarai.ac.at/traffic4cast/)

* 2020 https://www.iarai.ac.at/traffic4cast/2020-competition/
* 2019  https://www.iarai.ac.at/traffic4cast/2019-competition/

## Papers

### UrbanFM: Inferring Fine-Grained Urban Flows (KDD 2019)

Y. Liang *et al.*, “UrbanFM: Inferring Fine-Grained Urban Flows,” p. 11, 2019.



### Traffic Prediction in a Bike-Sharing System (SIGSPATIAL 2015)

Y. Li, Y. Zheng, H. Zhang, and L. Chen, “Traffic Prediction in a Bike-Sharing System,” p. 10.



### Traffic Flow Prediction With Big Data: A Deep Learning Approach (TITS 2015)

Y. Lv, Y. Duan, W. Kang, Z. Li, and F.-Y. Wang, “Traffic Flow Prediction With Big Data: A Deep Learning Approach,” *IEEE Trans. Intell. Transport. Syst.*, pp. 1–9, 2014, doi: [10.1109/TITS.2014.2345663](https://doi.org/10.1109/TITS.2014.2345663).



### Traffic Flow Prediction via Spatial Temporal Graph Neural Network (WWW 2020)

X. Wang *et al.*, “Traffic Flow Prediction via Spatial Temporal Graph Neural Network,” in *Proceedings of The Web Conference 2020*, Taipei Taiwan, Apr. 2020, pp. 1082–1092, doi: [10.1145/3366423.3380186](https://doi.org/10.1145/3366423.3380186).



### The Simpler The Better: A Unified Approach to Predicting Original Taxi Demands based on Large-Scale Online Platforms (KDD 2017)

Y. Tong *et al.*, “The Simpler The Better: A Unified Approach to Predicting Original Taxi Demands based on Large-Scale Online Platforms,” in *Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining - KDD ’17*, Halifax, NS, Canada, 2017, pp. 1653–1662, doi: [10.1145/3097983.3098018](https://doi.org/10.1145/3097983.3098018).



### STG2Seq: Spatial-Temporal Graph to Sequence Model for Multi-step Passenger Demand Forecasting (IJCAI 2019)

L. Bai, L. Yao, S. S. Kanhere, X. Wang, and Q. Z. Sheng, “STG2Seq: Spatial-Temporal Graph to Sequence Model for Multi-step Passenger Demand Forecasting,” in *Proceedings of the Twenty-Eighth International Joint Conference on Artificial Intelligence*, Macao, China, Aug. 2019, pp. 1981–1987, doi: [10.24963/ijcai.2019/274](https://doi.org/10.24963/ijcai.2019/274).



### Spatiotemporal Periodical Pattern Mining in Traffic Data (KDD 2013)

T. Jindal, P. Giridhar, L.-A. Tang, J. Li, and J. Han, “Spatiotemporal Periodical Pattern Mining in Traffic Data,” p. 8.



### Spatiotemporal Multi-Graph Convolution Network for Ride-Hailing Demand Forecasting (AAAI 2019)

X. Geng *et al.*, “Spatiotemporal Multi-Graph Convolution Network for Ride-Hailing Demand Forecasting,” *AAAI*, vol. 33, pp. 3656–3663, Jul. 2019, doi: [10.1609/aaai.v33i01.33013656](https://doi.org/10.1609/aaai.v33i01.33013656).



### Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting (IJCAI 2018)

B. Yu, H. Yin, and Z. Zhu, “Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting,” in *Proceedings of the Twenty-Seventh International Joint Conference on Artificial Intelligence*, Stockholm, Sweden, Jul. 2018, pp. 3634–3640, doi: [10.24963/ijcai.2018/505](https://doi.org/10.24963/ijcai.2018/505).



### Spatio-Temporal Graph Convolutional and Recurrent Networks for Citywide Passenger Demand Prediction (CIKM 2019)

L. Bai, L. Yao, S. S. Kanhere, X. Wang, W. Liu, and Z. Yang, “Spatio-Temporal Graph Convolutional and Recurrent Networks for Citywide Passenger Demand Prediction,” in *Proceedings of the 28th ACM International Conference on Information and Knowledge Management*, Beijing China, Nov. 2019, pp. 2293–2296, doi: [10.1145/3357384.3358097](https://doi.org/10.1145/3357384.3358097).



### Short-term speed predictions exploiting big data on large urban road networks (Transportation Research Part C: Emerging Technologies 2016)

G. Fusco, “Short-term speed predictions exploiting big data on large urban road networks,” p. 19, 2016.

### Short-term forecasting of passenger demand under on-demand ride services: A spatio-temporal deep learning approach (Transportation Research Part C: Emerging Technologies  2017)

J. Ke, H. Zheng, H. Yang, and X. (Michael) Chen, “Short-term forecasting of passenger demand under on-demand ride services: A spatio-temporal deep learning approach,” *Transportation Research Part C: Emerging Technologies*, vol. 85, pp. 591–608, Dec. 2017, doi: [10.1016/j.trc.2017.10.016](https://doi.org/10.1016/j.trc.2017.10.016).



### Regions, Periods, Activities: Uncovering Urban Dynamics via Cross-Modal Representation Learning (WWW 2017)

C. Zhang *et al.*, “Regions, Periods, Activities: Uncovering Urban Dynamics via Cross-Modal Representation Learning,” in *Proceedings of the 26th International Conference on World Wide Web*, Perth Australia, Apr. 2017, pp. 361–370, doi: [10.1145/3038912.3052601](https://doi.org/10.1145/3038912.3052601).



### Predicting citywide crowd flows using deep spatio-temporal residual networks (Artificial Intelligence 2018)

J. Zhang, Y. Zheng, D. Qi, R. Li, X. Yi, and T. Li, “Predicting citywide crowd flows using deep spatio-temporal residual networks,” *Artificial Intelligence*, vol. 259, pp. 147–166, Jun. 2018, doi: [10.1016/j.artint.2018.03.002](https://doi.org/10.1016/j.artint.2018.03.002).



### PRED: Periodic Region Detection for Mobility Modeling of Social Media Users (WSDM 2017)

Q. Yuan, W. Zhang, C. Zhang, X. Geng, G. Cong, and J. Han, “PRED: Periodic Region Detection for Mobility Modeling of Social Media Users,” in *Proceedings of the Tenth ACM International Conference on Web Search and Data Mining*, Cambridge United Kingdom, Feb. 2017, pp. 263–272, doi: [10.1145/3018661.3018680](https://doi.org/10.1145/3018661.3018680).



### Periodic-CRN: A Convolutional Recurrent Model for Crowd Density Prediction with Recurring Periodic Patterns (IJCAI 2018)

A. Zonoozi, J. Kim, X.-L. Li, and G. Cong, “Periodic-CRN: A Convolutional Recurrent Model for Crowd Density Prediction with Recurring Periodic Patterns,” in *Proceedings of the Twenty-Seventh International Joint Conference on Artificial Intelligence*, Stockholm, Sweden, Jul. 2018, pp. 3732–3738, doi: [10.24963/ijcai.2018/519](https://doi.org/10.24963/ijcai.2018/519).



### Multi-level Attention Networks for Multi-step Citywide Passenger Demands Prediction (TKDE 2019)

X. Zhou, Y. Shen, L. Huang, T. Zang, and Y. Zhu, “Multi-level Attention Networks for Multi-step Citywide Passenger Demands Prediction,” *IEEE Trans. Knowl. Data Eng.*, pp. 1–1, 2019, doi: [10.1109/TKDE.2019.2948005](https://doi.org/10.1109/TKDE.2019.2948005).





### Mobility Modeling and Prediction in Bike-Sharing Systems (MobiSys 2016)

Z. Yang, J. Hu, Y. Shu, P. Cheng, J. Chen, and T. Moscibroda, “Mobility Modeling and Prediction in Bike-Sharing Systems,” in *Proceedings of the 14th Annual International Conference on Mobile Systems, Applications, and Services*, Singapore Singapore, Jun. 2016, pp. 165–178, doi: [10.1145/2906388.2906408](https://doi.org/10.1145/2906388.2906408).



### Matrix Factorization for Spatio-Temporal Neural Networks with Applications to Urban Flow Prediction (CIKM 2019)

Z. Pan, Z. Wang, W. Wang, Y. Yu, J. Zhang, and Y. Zheng, “Matrix Factorization for Spatio-Temporal Neural Networks with Applications to Urban Flow Prediction,” in *Proceedings of the 28th ACM International Conference on Information and Knowledge Management - CIKM ’19*, Beijing, China, 2019, pp. 2683–2691, doi: [10.1145/3357384.3357832](https://doi.org/10.1145/3357384.3357832).



### Learning Traffic as Images: A Deep Convolutional Neural Network for Large-Scale Transportation Network Speed Prediction (Sensors 2017)

X. Ma, Z. Dai, Z. He, J. Ma, Y. Wang, and Y. Wang, “Learning Traffic as Images: A Deep Convolutional Neural Network for Large-Scale Transportation Network Speed Prediction,” *Sensors*, vol. 17, no. 4, p. 818, Apr. 2017, doi: [10.3390/s17040818](https://doi.org/10.3390/s17040818).



### Learning Dynamic Context Graphs for Predicting Social Events (KDD 2019)

S. Deng, H. Rangwala, and Y. Ning, “Learning Dynamic Context Graphs for Predicting Social Events,” in *Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining*, Anchorage AK USA, Jul. 2019, pp. 1007–1016, doi: [10.1145/3292500.3330919](https://doi.org/10.1145/3292500.3330919).



### GeoMAN: Multi-level Attention Networks for Geo-sensory Time Series Prediction (IJCAI 2018)

Y. Liang, “GeoMAN: Multi-level Attention Networks for Geo-sensory Time Series Prediction,” *Air Quality*, p. 7.



### Flow Prediction in Spatio-Temporal Networks Based on Multitask Deep Learning (TKDE 2019)

J. Zhang, Y. Zheng, J. Sun, and D. Qi, “Flow Prediction in Spatio-Temporal Networks Based on Multitask Deep Learning,” *IEEE Trans. Knowl. Data Eng.*, pp. 1–1, 2019, doi: [10.1109/TKDE.2019.2891537](https://doi.org/10.1109/TKDE.2019.2891537).



### FCCF: forecasting citywide crowd flows based on big data (SIGSPACIAL 2016)

M. X. Hoang, Y. Zheng, and A. K. Singh, “FCCF: forecasting citywide crowd flows based on big data,” in *Proceedings of the 24th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems - GIS ’16*, Burlingame, California, 2016, pp. 1–10, doi: [10.1145/2996913.2996934](https://doi.org/10.1145/2996913.2996934).



### DNN-Based Prediction Model for Spatial-Temporal Data (SIGSPACIAL 2016)

J. Zhang, Y. Zheng, D. Qi, R. Li, and X. Yi, “DNN-Based Prediction Model for Spatial-Temporal Data,” p. 4.



### Diffusion Convolutional Recurrent Neural Network: Data-Driven Traffic Forecasting (ICLR 2018)

Y. Li, R. Yu, C. Shahabi, and Y. Liu, “DIFFUSION CONVOLUTIONAL RECURRENT NEURAL NETWORK: DATA-DRIVEN TRAFFIC FORECASTING,” p. 16, 2018.



### DeepSTN+: Context-Aware Spatial-Temporal Neural Network for Crowd Flow Prediction in Metropolis (AAAI 2019)

Z. Lin, J. Feng, Z. Lu, Y. Li, and D. Jin, “DeepSTN+: Context-Aware Spatial-Temporal Neural Network for Crowd Flow Prediction in Metropolis,” *AAAI*, vol. 33, pp. 1020–1027, Jul. 2019, doi: [10.1609/aaai.v33i01.33011020](https://doi.org/10.1609/aaai.v33i01.33011020).



### DeepSD: Supply-Demand Prediction for Online Car-Hailing Services Using Deep Neural Networks (ICDE 2017)

D. Wang, W. Cao, J. Li, and J. Ye, “DeepSD: Supply-Demand Prediction for Online Car-Hailing Services Using Deep Neural Networks,” in *2017 IEEE 33rd International Conference on Data Engineering (ICDE)*, San Diego, CA, USA, Apr. 2017, pp. 243–254, doi: [10.1109/ICDE.2017.83](https://doi.org/10.1109/ICDE.2017.83).



### DeepPF: A deep learning based architecture for metro passenger flow prediction (Transportation Research Part C: Emerging Technologies)

Y. Liu, “DeepPF_ A deep learning based architecture for metro passenger flow prediction,” p. 17, 2019.

Transportation Research Part C Emerging Technologies



### Deep Multi-View Spatial-Temporal Network for Taxi Demand Prediction (AAAI 2018)

H. Yao *et al.*, “Deep Multi-View Spatial-Temporal Network for Taxi Demand Prediction,” p. 8.



### Deep Learning: A Generic Approach for Extreme Condition Traffic Forecasting (SDM 2017)

R. Yu, Y. Li, C. Shahabi, U. Demiryurek, and Y. Liu, “Deep Learning: A Generic Approach for Extreme Condition Traffic Forecasting,” 2017, doi: [10.1137/1.9781611974973.87](https://doi.org/10.1137/1.9781611974973.87).



### CityTraffic: Modeling Citywide Traffic via Neural Memorization and Generalization Approach (CIKM 2019)

X. Yi, Z. Duan, T. Li, T. Li, J. Zhang, and Y. Zheng, “CityTraffic: Modeling Citywide Traffic via Neural Memorization and Generalization Approach,” in *Proceedings of the 28th ACM International Conference on Information and Knowledge Management - CIKM ’19*, Beijing, China, 2019, pp. 2665–2671, doi: [10.1145/3357384.3357822](https://doi.org/10.1145/3357384.3357822).



### CityMomentum: an online approach for crowd behavior prediction at a citywide level (UbiComp 2015)

Z. Fan, X. Song, R. Shibasaki, and R. Adachi, “CityMomentum: an online approach for crowd behavior prediction at a citywide level,” in *Proceedings of the 2015 ACM International Joint Conference on Pervasive and Ubiquitous Computing - UbiComp ’15*, Osaka, Japan, 2015, pp. 559–569, doi: [10.1145/2750858.2804277](https://doi.org/10.1145/2750858.2804277).



### Bike Flow Prediction with Multi-Graph Convolutional Networks (SIGSPATIAL 2018)

D. Chai, L. Wang, and Q. Yang, “Bike Flow Prediction with Multi-Graph Convolutional Networks,” *arXiv:1807.10934 [cs, stat]*, Jul. 2018, Accessed: Oct. 16, 2019. [Online]. Available: http://arxiv.org/abs/1807.10934.





### Adaptive Graph Convolutional Recurrent Network for Trafﬁc Forecasting (NeurIPS 2020)

L. Bai, L. Yao, and C. Li, “Adaptive Graph Convolutional Recurrent Network for Trafﬁc Forecasting,” p. 12.



### A spatiotemporal correlative k-nearest neighbor model for short-term traffic multistep forecasting (Transportation Research Part C: Emerging Technologies)

P. Cai, Y. Wang, G. Lu, P. Chen, C. Ding, and J. Sun, “A spatiotemporal correlative k-nearest neighbor model for short-term traffic multistep forecasting,” *Transportation Research Part C: Emerging Technologies*, vol. 62, pp. 21–34, Jan. 2016, doi: [10.1016/j.trc.2015.11.002](https://doi.org/10.1016/j.trc.2015.11.002).



### A Dual-Stage Attention-Based Recurrent Neural Network for Time Series Prediction (IJCAI 2017)

” in *Proceedings of the Twenty-Sixth International Joint Conference on Artificial Intelligence*, Melbourne, Australia, Aug. 2017, pp. 2627–2633, doi: [10.24963/ijcai.2017/366](https://doi.org/10.24963/ijcai.2017/366).



### Spatial-Temporal Fusion Graph Neural Networks for Traffic Flow Forecasting (AAAI 2021)

