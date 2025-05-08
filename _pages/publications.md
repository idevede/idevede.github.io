---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}

  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>

{% endif %}


{% include base_path %}


{% for post in site.publications reversed %}

  {% include archive-single.html %}

{% endfor %}

## Selected Topic: Time Series Foundation Model:

1. **TEMPO: Prompt-based generative pre-trained transformer for time series forecasting**  
   **Defu Cao**, Furong Jia, Sercan O Arik, Tomas Pfister, Yixiang Zheng, Wen Ye, Yan Liu  
   *[ICLR 2024](https://iclr.cc/)* | [paper](https://arxiv.org/pdf/2310.04948) | [code](https://github.com/DC-research/TEMPO) | [huggingface](https://huggingface.co/Melady/TEMPO)

2. **TimeDiT: General-purpose Diffusion Transformers for Time Series Foundation Model**  
   **Defu Cao**, Wen Ye, Yizhou Zhang, Yan Liu  
   *[Arxiv 2024](https://arxiv.org/abs/2409.02322)* | [paper](https://arxiv.org/abs/2409.02322)

3. **GPT4MTS: Prompt-based Large Language Model for Multimodal Time-series Forecasting**  
   Furong Jia, Kevin Wang, Yixiang Zheng, **Defu Cao**, Yan Liu  
   *[AAAI/EAAI 2024](https://aaai.org/conference/aaai/aaai-24/)* | [paper](https://ojs.aaai.org/index.php/AAAI/article/view/30383) | [Multimodal Dataset](https://drive.google.com/file/d/1mGgY9dl3QHFVHcR4Rm6mbg3p8RwYtMdU/view?usp=sharing)

4. **Beyond Forecasting: Compositional Time Series Reasoning for End-to-End Task Execution**  
   Wen Ye, Yizhou Zhang, Wei Yang, Lumingyuan Tang, **Defu Cao**, Jie Cai, Yan Liu  
   *[Arxiv 2024](https://arxiv.org/abs/2410.04047)* | [paper](https://ojs.aaai.org/index.php/AAAI/article/view/30383)

### Survey Papers:

1. **When Physics Meets Machine Learning: A Survey of Physics-Informed Machine Learning**  
   Chuizheng Meng, Sungyong Seo, **Defu Cao**, Sam Griesemer, Yan Liu  
   *[Arxiv 2022](https://arxiv.org/abs/2203.16797)* | [paper](https://arxiv.org/abs/2203.16797)

### Conference Papers:

1. **SVGformer: Representation Learning for Continuous Vector Graphics using Transformers**  
   **Defu Cao**, Zhaowen Wang, Jose Echevarria, Yan Liu  
   *[CVPR 2023](https://cvpr.thecvf.com/)* | [paper](hhttps://openreview.net/forum?id=NA2HCcGbLAd)

2. **Coupled Multiwavelet Neural Operator Learning for Coupled Partial Differential Equations**  
   Xiongye Xiao, **Defu Cao**, Ruochen Yang, Gaurav Gupta, Gengshuo Liu, Chenzhong Yin, Radu Balan, Paul Bogdan  
   *[ICLR 2023](https://iclr.cc/)* | [paper](https://arxiv.org/abs/2303.02304)

3. **Time-delayed Multivariate Time Series Predictions**  
   Hao Niu, Guillaume Habault, Roberto Legaspi, Chuizheng Meng, **Defu Cao**, Shinya Wada, Chihiro Ono, Yan Liu  
   *[SDM 2023](https://www.siam.org/conferences/cm/conference/sdm23)*

4. **Estimating Treatment Effects from Irregular Time Series Observations with Hidden Confounders**  
   **Defu Cao**, James Enouen, Yujing Wang, Xiangchen Song, Chuizheng Meng, Hao Niu, Yan Liu  
   *[AAAI 2023](https://aaai.org/Conferences/AAAI-23/aaai23call/)* | [paper](https://arxiv.org/abs/2303.02320)

5. **Counterfactual Neural Temporal Point Process for Estimating Causal Influence of Misinformation on Social Media**  
   Yizhou Zhang, **Defu Cao**, Yan Liu  
   *[NeurIPS 2022](https://neurips.cc/)* | [paper](https://arxiv.org/abs/2210.07518) | [code](https://github.com/yizhouzhang97/CNTPP)

6. **Hardware Reusability Optimization for High-Level Synthesis of Component-Based Processors**  
   Xianhua Liu, **Defu Cao**, Qinshu Chen  
   *[IEEE ICCCAS 2022](http://www.icccas.org/)* | [paper](https://ieeexplore.ieee.org/document/9825407)

7. **Enhancing Self-Attention with Knowledge-Assisted Attention Maps**  
   Jiangang Bai, Yujing Wang, Hong Sun, Ruonan Wu, Tianmeng Yang, Pengfei Tang, Wei Shen, **Defu Cao**, Mingliang Zhang, Yaming Yang, Jing Bai, Yunhai Tong, Hao Sun, Ruofei Zhang  
   *[NAACL 2022](https://2022.naacl.org/)* | [paper](https://aclanthology.org/2022.naacl-main.8/)

8. **Mu2ReST: Multi-Resolution Recursive Spatio-Temporal Transformer for Long-Term Prediction**  
   Hao Niu, Chuizheng Meng, **Defu Cao**, Guillaume Habault, Roberto Legaspi, Shinya Wada, Chihiro Ono, Yan Liu  
   *[PAKDD 2022](http://pakdd.net/)* | [paper](https://dl.acm.org/doi/abs/10.1007/978-3-031-05933-9_6)

9. **Spectral Temporal Graph Neural Network for Trajectory Prediction**  
   **Defu Cao**, Jiachen Li, Hengbo Ma, Masayoshi Tomizuka  
   *[ICRA 2021](https://www.ieee-icra.org/)* | [paper](https://arxiv.org/abs/2106.02930)

10. **Spectral temporal graph neural network for multivariate time-series forecasting**  
    **Defu Cao**, Yujing Wang, Juanyong Duan, Ce Zhang, Xia Zhu, Conguri Huang, Yunhai Tong, Bixiong Xu, Jing Bai, Jie Tong, Qi Zhang  
    *[NeurIPS 2020](https://nips.cc/Conferences/2021/)* | [paper](https://arxiv.org/abs/2103.07719) | [code](https://github.com/microsoft/StemGNN) | [video](https://slideslive.at/38937983/spectral-temporal-graph-neural-network-for-multivariate-timeseries-forecasting?ref=speaker-18146-latest) | **Spotlight (2%)**

11. **Multivariate time-series anomaly detection via graph attention network**  
    Hang Zhao, Yujing Wang, Juanyong Duan, Congrui Huang, **Defu Cao**, Yunhai Tong, Bixiong Xu, Jing Bai, Jie Tong, Qi Zhang  
    *[ICDM 2020](http://icdm2020.bigke.org/)* | [paper](https://arxiv.org/abs/2009.02040) | [code](https://github.com/mangushev/mtad-gat)

12. **FTCLNet: Convolutional LSTM with Fourier Transform for Vulnerability Detection**  
    **Defu Cao**, Jing Huang, Xuanyu Zhang, Xianhua Liu  
    *[TrustCom 2020](http://www.ieee-trustcom.org/TrustCom2020/)* | [paper](https://ieeexplore.ieee.org/abstract/document/9343188)

### Workshop Papers:

1. **DSLOB: A Synthetic Limit Order Book Dataset for Benchmarking Forecasting Algorithms under Distributional Shift**  
   **Defu Cao**, Yousef El-Laham, Loc Trinh, Svitlana Vyetrenko, Yan Liu  
   *[NeurIPS 2022](https://openreview.net/forum?id=_u-1--wBV1)* | [paper](https://arxiv.org/abs/2211.11513) | [Proposed Dataset](mailto:defucao@usc.edu)

2. **Estimating Treatment Effects in Continuous Time with Hidden Confounders**  
   **Defu Cao**, James Enouen, Yan Liu  
   *[ICML 2022](https://sites.google.com/view/continuous-time-methods-icml/home)* | [video](https://icml.cc/virtual/2022/workshop/13452#wse-detail-18710) | [paper](https://arxiv.org/abs/2302.09446)


## Publication Impact

<div class="citation-map-container">
  <iframe src="{{ site.baseurl }}/citation_map.html" width="100%" height="500" frameborder="0"></iframe>
</div>
