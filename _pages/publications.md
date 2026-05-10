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

## Selected Research Map

| Research Stack | Representative Papers | Positioning |
| --- | --- | --- |
| **Post-training and agentic systems** | TSOrchestra, HILA, TS-Reasoner | R1-style fine-tuning, metacognitive policy optimization, tool use, feedback loops, and human-agent collaboration. |
| **LLM safety and agent security** | "Someone Hid It!", Topology Matters | Robustness and privacy risks in LLM retrieval, RAG, agent memory, and multi-agent communication topology. |
| **Foundation models for structured and scientific data** | TEMPO, ClimateLLM, TimeDiT, PINFDiT | Pretraining and generative modeling for complex numerical, spatiotemporal, weather, and physics-constrained data. |
| **Numerical interfaces for LLMs** | Speaking Numbers to LLMs, GPT4MTS | Representation and prompting layers that let language models consume continuous values, multimodal signals, and numerical structure. |
| **Benchmarks and high-stakes evaluation** | TSAIA, TemporalBench, ECG benchmark, waveform reasoning | Diagnostic evaluation for whether LLM/agent systems reason reliably under contextual, event-driven, and clinical constraints. |
| **AI policy and governance collaboration** | Cooperative AI policymaking platform | Open-source collaboration on policy interfaces, economic forecasting, and public-value elicitation. |
| **Surveys and research frameworks** | Reasoning and agentic systems survey, physics-informed ML survey, Toward Evolutionary Intelligence | Field-level organization, taxonomies, and design principles. |

## Post-Training and Agentic Systems

1. **Conversational Time Series Foundation Models: Towards Explainable and Effective Forecasting**<br>
   **Defu Cao**, Michael Gee, Jinbo Liu, Hengxuan Wang, Wei Yang, Rui Wang, Yan Liu<br>
   *arXiv 2025* | [paper](https://arxiv.org/abs/2512.16022) | [code](https://github.com/DC-research/TSorchestra)<br>
   *Positioning:* TSOrchestra; R1-style fine-tuned LLM judge that explains and orchestrates foundation-model ensembles through multi-turn optimization.

2. **Adaptive Collaboration with Humans: Metacognitive Policy Optimization for Multi-Agent LLMs with Continual Learning**<br>
   Wei Yang, **Defu Cao**, Jiacheng Pang, Muyan Weng, Yan Liu<br>
   *[ICLR 2026](https://iclr.cc/)* | [paper](https://openreview.net/forum?id=IKVUB9Exuc) |[code](https://github.com/USC-Melady/HILA) <br>
   *Positioning:* HILA; post-training for human-agent collaboration through GRPO-based metacognitive deferral and continual learning from expert feedback.

3. **TS-Reasoner: Domain-Oriented Time Series Inference Agents for Reasoning and Automated Analysis**<br>
   Wen Ye, Wei Yang, **Defu Cao**, Yizhou Zhang, Lumingyuan Tang, Jie Cai, Yan Liu<br>
   *TMLR, March 2026* | [OpenReview](https://openreview.net/forum?id=yhy7Vigjcf) | [code](https://github.com/wen-ye-xwz/TS-Reasoner)<br>
   *Positioning:* domain-specialized inference agent accepted by TMLR after Action Editor confirmation; combines LLM reasoning, computational tools, and an error-feedback loop for multi-step analytical workflows.

## LLM Safety and Agent Security

1. **"Someone Hid It!": Query-Agnostic Black-Box Attacks on LLM-Based Retrieval**<br>
   Jiate Li, **Defu Cao**, Li Li, Wei Yang, Yuehan Qin, Chenxiao Yu, Tiannuo Yang, Ryan A. Rossi, Yan Liu, Xiyang Hu, Yue Zhao<br>
   *[ICML 2026](https://icml.cc/)* | [paper](https://arxiv.org/abs/2602.00364)<br>
   *Positioning:* query-agnostic, black-box adversarial attacks for LLM-based retrieval, including RAG, dense IR, and agent memory retrieval.

2. **Topology Matters: Measuring Memory Leakage in Multi-Agent LLMs**<br>
   Jinbo Liu, **Defu Cao**, Yifei Wei, Tianyao Su, Yuan Liang, Yushun Dong, Yan Liu, Yue Zhao, Xiyang Hu<br>
   *arXiv 2025* | [paper](https://arxiv.org/abs/2512.04668)<br>
   *Positioning:* multi-agent privacy and security; measures how communication graph topology affects PII leakage from agent memory.

## Foundation Models for Structured and Scientific Data

1. **TEMPO: Prompt-based Generative Pre-trained Transformer for Time Series Forecasting**<br>
   **Defu Cao**, Furong Jia, Sercan O Arik, Tomas Pfister, Yixiang Zheng, Wen Ye, Yan Liu<br>
   *[ICLR 2024](https://iclr.cc/)* | [paper](https://arxiv.org/abs/2310.04948) | [code](https://github.com/DC-research/TEMPO) | [huggingface](https://huggingface.co/Melady/TEMPO)<br>
   *Positioning:* GPT-style pretraining with decomposition and prompting for transferable numerical sequence modeling.

2. **ClimateLLM: Efficient Weather Forecasting via Frequency-Aware Large Language Models**<br>
   Shixuan Li, Wei Yang, Peiyu Zhang, Xiongye Xiao, **Defu Cao**, Yuehan Qin, Xiaole Zhang, Yue Zhao, Paul Bogdan<br>
   *arXiv 2025* | [paper](https://arxiv.org/abs/2502.11059)<br>
   *Positioning:* frequency-aware LLM foundation model for weather, combining Fourier decomposition, MoE routing, and cross-spatial/cross-temporal prompting.

3. **TimeDiT: General-purpose Diffusion Transformers for Time Series Foundation Model**<br>
   **Defu Cao**, Wen Ye, Yizhou Zhang, Yan Liu<br>
   *ICML 2024 Workshop on Foundation Models in the Wild* | [paper](https://arxiv.org/abs/2409.02322)<br>
   *Positioning:* diffusion-transformer proto-foundation model for probabilistic generation, imputation, forecasting, anomaly detection, and model editing.

4. **PINFDiT: Energy-Based Physics-Informed Diffusion Transformers for General-purpose Time Series Tasks**<br>
   **Defu Cao**, Wen Ye, Yizhou Zhang, Sam Griesemer, Yan Liu<br>
   *[ICLR 2026](https://iclr.cc/)* | [paper](https://openreview.net/forum?id=EphTlUJ4XN)<br>
   *Positioning:* physics-guided inference for diffusion foundation models, using calibrated Langevin correction to enforce physical consistency without retraining.

## Numerical Interfaces for LLMs

1. **Speaking Numbers to LLMs: Multi-Wavelet Number Embeddings for Time Series Forecasting**<br>
   **Defu Cao**, Zijie Lei, Jiao Sun, Yan Liu<br>
   *[IJCAI 2026](https://www.ijcai.org/)* | [paper](https://openreview.net/pdf?id=mk2ADdNQAI)<br>
   *Positioning:* not a standalone foundation-model pretraining paper; it is a numerical representation layer. Multi-Wavelet Number Embedding (MWNE) decomposes continuous values with wavelet bases so LLMs preserve digit recovery, numeracy, multi-scale structure, and normalization robustness.

2. **GPT4MTS: Prompt-based Large Language Model for Multimodal Time-series Forecasting**<br>
   Furong Jia, Kevin Wang, Yixiang Zheng, **Defu Cao**, Yan Liu<br>
   *[AAAI/EAAI 2024](https://aaai.org/conference/aaai/aaai-24/)* | [paper](https://doi.org/10.1609/aaai.v38i21.30383) | [Multimodal Dataset](https://drive.google.com/file/d/1mGgY9dl3QHFVHcR4Rm6mbg3p8RwYtMdU/view?usp=sharing)<br>
   *Positioning:* prompt-based adaptation of LLMs for multimodal numerical forecasting.

## AI Policy and Governance Collaboration

1. **Creating a Cooperative AI Policymaking Platform through Open Source Collaboration**<br>
   Aiden Lewington, Alekhya Vittalam, Anshumaan Singh, Anuja Uppuluri, Arjun Ashok, Ashrith Mandayam Athmaram, Austin Milt, Benjamin Smith, Charlie Weinberger, Chatanya Sarin, Christoph Bergmeir, Cliff Chang, Daivik Patel, Daniel Li, David Bell, **Defu Cao**, et al.<br>
   *arXiv 2024* | [paper](https://arxiv.org/abs/2412.06936) | [organization](https://humun.org/get-involved)<br>
   *Positioning:* large open-source collaboration with Humanity Unleashed on a cooperative AI policymaking platform; contributed to the foundation-model/pretraining component.

## Benchmarks and High-Stakes Evaluation

1. **When LLM Meets Time Series: Can LLMs Perform Multi-Step Time Series Reasoning and Inference**<br>
   Wen Ye, Jinbo Liu, **Defu Cao**, Wei Yang, Yan Liu<br>
   *arXiv 2025* | [paper](https://arxiv.org/abs/2509.01822)<br>
   *Positioning:* TSAIA benchmark for evaluating LLMs as domain assistants over multi-step numerical analysis tasks.

2. **TemporalBench: A Benchmark for Evaluating LLM-Based Agents on Contextual and Event-Informed Time Series Tasks**<br>
   Muyan Weng, **Defu Cao**, Wei Yang, Yashaswi Sharma, Yan Liu<br>
   *arXiv 2026* | [paper](https://arxiv.org/abs/2602.13272)<br>
   *Positioning:* diagnostic benchmark for contextual and event-conditioned reasoning, separating forecasting accuracy from temporal understanding.

3. **Position: Beyond Prediction: Toward Verifiable Physiological Waveform Reasoning with Foundation Models and Agentic LLMs**<br>
   Xiaoda Wang, Ching Chang, **Defu Cao**, Kaiqiao Han, Fang Sun, Yue Huang, Minxiao Wang, Chang Xu, Xiao Luo, Runze Yan, Xiangliang Zhang, Xiao Hu, Yan Liu, Yizhou Sun, Wei Wang, Carl Yang<br>
   *[ICML 2026](https://icml.cc/)* | [paper](https://openreview.net/forum?id=cgpU6fhUXx)<br>
   *Positioning:* high-stakes Physiological Waveform Reasoning; argues for verifiable Plan-Act-Verify systems that connect localized signal evidence to clinical decisions.

4. **EnECG: Efficient Ensemble Learning for Electrocardiogram Multi-task Foundation Model**<br>
   Yuhao Xu, Xiaoda Wang, Jiaying Lu, Sirui Ding, **Defu Cao**, Huaxiu Yao, Yan Liu, Xiao Hu, Carl Yang<br>
   *arXiv 2025* | [paper](https://arxiv.org/abs/2511.22935)<br>
   *Positioning:* efficient ensemble and MoE adaptation for ECG multi-task foundation models.

5. **An Electrocardiogram Multi-task Benchmark with Comprehensive Evaluations and Insightful Findings**<br>
   Yuhao Xu, Jiaying Lu, Sirui Ding, **Defu Cao**, Xiao Hu, Carl Yang<br>
   *arXiv 2025* | [paper](https://arxiv.org/abs/2512.08954)<br>
   *Positioning:* benchmark asking whether language, general time-series, and ECG foundation models are useful for ECG analysis.

## Surveys and Research Frameworks

1. **A Survey of Reasoning and Agentic Systems in Time Series with Large Language Models**<br>
   Ching Chang, Yidan Shi, **Defu Cao**, Wei Yang, Jeehyun Hwang, Haixin Wang, Jiacheng Pang, Wei Wang, Yan Liu, Wen-Chih Peng, Tien-Fu Chen<br>
   *arXiv 2025* | [paper](https://arxiv.org/abs/2509.11575) | [repo](https://github.com/blacksnail789521/Time-Series-Reasoning-Survey)<br>
   *Positioning:* actual survey; organizes reasoning topologies, tool use, evidence grounding, benchmarks, and agent loops for temporal data.

2. **Toward Evolutionary Intelligence: LLM-based Agentic Systems with Multi-Agent Reinforcement Learning**<br>
   Wei Yang, Muyan Weng, Jiacheng Pang, **Defu Cao**, Heng Ping, Peiyu Zhang, Shixuan Li, Yue Zhao, Qiang Yang, Mengdi Wang, Yan Liu<br>
   *SSRN 2026* | [paper](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5819182)<br>
   *Positioning:* research framework for learning paradigms in LLM-based multi-agent systems, especially MARL-driven adaptive and evolutionary agent societies.

3. **When Physics Meets Machine Learning: A Survey of Physics-Informed Machine Learning**<br>
   Chuizheng Meng, Sungyong Seo, **Defu Cao**, Sam Griesemer, Yan Liu<br>
   *arXiv 2022* | [paper](https://arxiv.org/abs/2203.16797)<br>
   *Positioning:* actual survey of physics-informed machine learning.

## Selected Publications

### 2026

1. **TS-Reasoner: Domain-Oriented Time Series Inference Agents for Reasoning and Automated Analysis**<br>
   Wen Ye, Wei Yang, **Defu Cao**, Yizhou Zhang, Lumingyuan Tang, Jie Cai, Yan Liu<br>
   *TMLR, March 2026* | [OpenReview](https://openreview.net/forum?id=yhy7Vigjcf) | [code](https://github.com/wen-ye-xwz/TS-Reasoner)

2. **"Someone Hid It!": Query-Agnostic Black-Box Attacks on LLM-Based Retrieval**<br>
   Jiate Li, **Defu Cao**, Li Li, Wei Yang, Yuehan Qin, Chenxiao Yu, Tiannuo Yang, Ryan A. Rossi, Yan Liu, Xiyang Hu, Yue Zhao<br>
   *[ICML 2026](https://icml.cc/)* | [paper](https://arxiv.org/abs/2602.00364)

3. **Position: Beyond Prediction: Toward Verifiable Physiological Waveform Reasoning with Foundation Models and Agentic LLMs**<br>
   Xiaoda Wang, Ching Chang, **Defu Cao**, Kaiqiao Han, Fang Sun, Yue Huang, Minxiao Wang, Chang Xu, Xiao Luo, Runze Yan, Xiangliang Zhang, Xiao Hu, Yan Liu, Yizhou Sun, Wei Wang, Carl Yang<br>
   *[ICML 2026](https://icml.cc/)* | [paper](https://openreview.net/forum?id=cgpU6fhUXx)

4. **Speaking Numbers to LLMs: Multi-Wavelet Number Embeddings for Time Series Forecasting**<br>
   **Defu Cao**, Zijie Lei, Jiao Sun, Yan Liu<br>
   *[IJCAI 2026](https://www.ijcai.org/)* | [paper](https://openreview.net/pdf?id=mk2ADdNQAI)

5. **PINFDiT: Energy-Based Physics-Informed Diffusion Transformers for General-purpose Time Series Tasks**<br>
   **Defu Cao**, Wen Ye, Yizhou Zhang, Sam Griesemer, Yan Liu<br>
   *[ICLR 2026](https://iclr.cc/)* | [paper](https://openreview.net/forum?id=EphTlUJ4XN)

6. **Adaptive Collaboration with Humans: Metacognitive Policy Optimization for Multi-Agent LLMs with Continual Learning**<br>
   Wei Yang, **Defu Cao**, Jiacheng Pang, Muyan Weng, Yan Liu<br>
   *[ICLR 2026](https://iclr.cc/)* | [paper](https://openreview.net/forum?id=IKVUB9Exuc)

7. **Orthogonalized estimation of difference of q-functions**<br>
   **Defu Cao**, Angela Zhou<br>
   *[AISTATS 2026](https://aistats.org/)* | [paper](https://arxiv.org/abs/2406.08697)

### 2024-2025

1. **Neuron-based Multifractal Analysis of Neuron Interaction Dynamics in Large Models**<br>
   Xiongye Xiao, Heng Ping, Chenyu Zhou, **Defu Cao**, Yaxing Li, Yizhuo Zhou, Shixuan Li, Nikos Kanakaris, Paul Bogdan<br>
   *[ICLR 2025](https://iclr.cc/)*

2. **When Splitting Makes Stronger: A Theoretical and Empirical Analysis of Divide-and-Conquer Prompting in LLMs**<br>
   Yizhou Zhang\*, **Defu Cao**\*, Yan Liu<br>
   *[CoLM 2025](https://colmweb.org/)*

3. **TEMPO: Prompt-based Generative Pre-trained Transformer for Time Series Forecasting**<br>
   **Defu Cao**, Furong Jia, Sercan O Arik, Tomas Pfister, Yixiang Zheng, Wen Ye, Yan Liu<br>
   *[ICLR 2024](https://iclr.cc/)* | [paper](https://arxiv.org/abs/2310.04948) | [code](https://github.com/DC-research/TEMPO) | [huggingface](https://huggingface.co/Melady/TEMPO)

4. **GPT4MTS: Prompt-based Large Language Model for Multimodal Time-series Forecasting**<br>
   Furong Jia, Kevin Wang, Yixiang Zheng, **Defu Cao**, Yan Liu<br>
   *[AAAI/EAAI 2024](https://aaai.org/conference/aaai/aaai-24/)* | [paper](https://doi.org/10.1609/aaai.v38i21.30383)

5. **Active Sequential Posterior Estimation for Sample-Efficient Simulation-Based Inference**<br>
   Sam Griesemer, **Defu Cao**, Zijun Cui, Carolina Osorio, Yan Liu<br>
   *[NeurIPS 2024](https://neurips.cc/)*

6. **An Empirical Examination of Balancing Strategy for Counterfactual Estimation on Time Series**<br>
   Qiang Huang, Chuizheng Meng, **Defu Cao**, Biwei Huang, Yi Chang, Yan Liu<br>
   *[ICML 2024](https://icml.cc/)*

7. **Neuro-Inspired Hierarchical Multimodal Learning**<br>
   Xiongye Xiao, Gengshuo Liu, Gaurav Gupta, **Defu Cao**, Shixuan Li, Yaxing Li, Tianqing Fang, Mingxi Cheng, Paul Bogdan<br>
   *[ICLR 2024](https://iclr.cc/)*

8. **MUGSI: Distilling GNNs with Multi-Granularity Structural Information for Graph Classification**<br>
   Tianjun Yao, Jiaqi Sun, **Defu Cao**, Kun Zhang, Guangyi Chen<br>
   *[WWW 2024](https://www2024.thewebconf.org/)* | [paper](https://dl.acm.org/doi/10.1145/3589334.3645550)

9. **Coupled Multiwavelet Neural Operator Learning for Coupled Partial Differential Equations**<br>
   Xiongye Xiao, **Defu Cao**, Ruochen Yang, Gaurav Gupta, Gengshuo Liu, Chenzhong Yin, Radu Balan, Paul Bogdan<br>
   *[ICLR 2024](https://iclr.cc/)* | [paper](https://arxiv.org/abs/2303.02304)

### 2023 and Earlier

1. **Large Scale Financial Time Series Forecasting with Multi-Faceted Model**<br>
   **Defu Cao**, Yixiang Zheng, Parisa Hassanzadeh, Simran Lamba, Xiaomo Liu, Yan Liu<br>
   *[ICAIF 2023](https://ai-finance.org/)* | **Oral** | [paper](https://dl.acm.org/doi/10.1145/3604237.3626886)

2. **SVGformer: Representation Learning for Continuous Vector Graphics using Transformers**<br>
   **Defu Cao**, Zhaowen Wang, Jose Echevarria, Yan Liu<br>
   *[CVPR 2023](https://cvpr.thecvf.com/)* | [paper](https://openaccess.thecvf.com/content/CVPR2023/html/Cao_SVGformer_Representation_Learning_for_Continuous_Vector_Graphics_Using_Transformers_CVPR_2023_paper.html)

3. **Time-delayed Multivariate Time Series Predictions**<br>
   Hao Niu, Guillaume Habault, Roberto Legaspi, Chuizheng Meng, **Defu Cao**, Shinya Wada, Chihiro Ono, Yan Liu<br>
   *[SDM 2023](https://www.siam.org/conferences/cm/conference/sdm23)*

4. **Estimating Treatment Effects from Irregular Time Series Observations with Hidden Confounders**<br>
   **Defu Cao**, James Enouen, Yujing Wang, Xiangchen Song, Chuizheng Meng, Hao Niu, Yan Liu<br>
   *[AAAI 2023](https://aaai.org/Conferences/AAAI-23/aaai23call/)* | [paper](https://arxiv.org/abs/2303.02320)

5. **Counterfactual Neural Temporal Point Process for Estimating Causal Influence of Misinformation on Social Media**<br>
   Yizhou Zhang, **Defu Cao**, Yan Liu<br>
   *[NeurIPS 2022](https://neurips.cc/)* | [paper](https://arxiv.org/abs/2210.07518) | [code](https://github.com/yizhouzhang97/CNTPP)

6. **Mu2ReST: Multi-Resolution Recursive Spatio-Temporal Transformer for Long-Term Prediction**<br>
   Hao Niu, Chuizheng Meng, **Defu Cao**, Guillaume Habault, Roberto Legaspi, Shinya Wada, Chihiro Ono, Yan Liu<br>
   *[PAKDD 2022](http://pakdd.net/)* | [paper](https://dl.acm.org/doi/abs/10.1007/978-3-031-05933-9_6)

7. **Enhancing Self-Attention with Knowledge-Assisted Attention Maps**<br>
   Jiangang Bai, Yujing Wang, Hong Sun, Ruonan Wu, Tianmeng Yang, Pengfei Tang, Wei Shen, **Defu Cao**, Mingliang Zhang, Yaming Yang, Jing Bai, Yunhai Tong, Hao Sun, Ruofei Zhang<br>
   *[NAACL 2022](https://2022.naacl.org/)* | [paper](https://aclanthology.org/2022.naacl-main.8/)

8. **Spectral Temporal Graph Neural Network for Trajectory Prediction**<br>
   **Defu Cao**, Jiachen Li, Hengbo Ma, Masayoshi Tomizuka<br>
   *[ICRA 2021](https://www.ieee-icra.org/)* | [paper](https://arxiv.org/abs/2106.02930)

9. **Spectral temporal graph neural network for multivariate time-series forecasting**<br>
   **Defu Cao**, Yujing Wang, Juanyong Duan, Ce Zhang, Xia Zhu, Conguri Huang, Yunhai Tong, Bixiong Xu, Jing Bai, Jie Tong, Qi Zhang<br>
   *[NeurIPS 2020](https://nips.cc/Conferences/2021/)* | [paper](https://arxiv.org/abs/2103.07719) | [code](https://github.com/microsoft/StemGNN) | [video](https://slideslive.at/38937983/spectral-temporal-graph-neural-network-for-multivariate-timeseries-forecasting?ref=speaker-18146-latest) | **Spotlight (2%)**

10. **Multivariate time-series anomaly detection via graph attention network**<br>
   Hang Zhao, Yujing Wang, Juanyong Duan, Congrui Huang, **Defu Cao**, Yunhai Tong, Bixiong Xu, Jing Bai, Jie Tong, Qi Zhang<br>
   *[ICDM 2020](http://icdm2020.bigke.org/)* | [paper](https://arxiv.org/abs/2009.02040) | [code](https://github.com/mangushev/mtad-gat)



### Workshop Papers:

1. **TimeDiT: General-purpose Diffusion Transformers for Time Series Foundation Model**<br>
   **Defu Cao**, Wen Ye, Yizhou Zhang, Yan Liu<br>
   *[ICML 2024 Workshop on Foundation Models in the Wild](https://icml.cc/)* | [paper](https://arxiv.org/abs/2409.02322)

2. **DSLOB: A Synthetic Limit Order Book Dataset for Benchmarking Forecasting Algorithms under Distributional Shift**<br>
   **Defu Cao**, Yousef El-Laham, Loc Trinh, Svitlana Vyetrenko, Yan Liu<br>
   *[NeurIPS 2022 DistShift Workshop](https://openreview.net/forum?id=_u-1--wBV1)* | [paper](https://arxiv.org/abs/2211.11513) | [Proposed Dataset](mailto:defucao@usc.edu)

3. **Estimating Treatment Effects in Continuous Time with Hidden Confounders**<br>
   **Defu Cao**, James Enouen, Yan Liu<br>
   *[ICML 2022](https://sites.google.com/view/continuous-time-methods-icml/home)* | [video](https://icml.cc/virtual/2022/workshop/13452#wse-detail-18710) | [paper](https://arxiv.org/abs/2302.09446)


### Patents:

1. **Representation Learning for Continuous Vector Graphics**<br>
   **Defu Cao**, Zhaowen Wang, Jose Echevarria
   *US Patent Application US20240303870A1* | Status: Published Patent Application, United States, 2024 | [USPTO](https://patents.google.com/patent/US20240303870A1/)

## Publication Impact

<div class="citation-map-container">
  <iframe src="{{ site.baseurl }}/citation_map.html" width="100%" height="500" frameborder="0"></iframe>
</div>
