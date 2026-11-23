---
title: "논문 인박스 — 2026-11-23"
updated: 2026-11-23
kind: papers
---

# 📬 논문 인박스 — 2026-11-23

> 새 논문 **19편** — 🆕 신간(최근 14일, 최신순) + ✅ 검증(최근 2년, 인용순). 🚧 = 내 막힌 길목과 닿는 논문.
> 세션에서 *"이번 주 새 논문 같이 보자"* 라고 하면 러너가 여기서 골라 준다.
> 다 읽을 필요 없다 — **제목과 초록만 훑고 1편만 골라** 깊게 보는 편이 낫다.

> ⚠️ **분야가 고정되지 않은 주제 4개** — Yoo, Hoi-Jun, On-device AI accelerator, Neural rendering and NeRF accelerator, Computing-in-memory and processing-in-memory
> 이 주제들은 단어로만 검색된다. 약어가 겹치면 엉뚱한 분야의 논문이 섞인다(`HBM` → high bandwidth memory / human breast milk).
> 세션에서 러너에게 **"이 주제 분야 고정해줘"** 라고 하면, 이미 읽은 논문을 씨앗으로 삼아 분야를 잡아 준다 — 사람이 코드를 찾을 필요는 없다.

## Yoo, Hoi-Jun

### 🆕 [Hardware Acceleration of Vision-Language-Action Models with Weight Precision Rising over the Flow Steps](https://doi.org/10.48550/arxiv.2611.24234)
<sub>2026-11-18 · Robin Geens, Simon Haepers, Jonas Crols 외 · arXiv (Cornell University)</sub>

> Vision-language-action (VLA) models such as GR00T control robots through an action head: a diffusion transformer that turns noise into a chunk of actions in a few flow-matching steps. Every step re-reads all of the head's weights from DRAM but applies each weight to only about fifty tokens. Inference is therefore memory-bound, and its latency and energy are largely determined by the total number o

### 🆕 [Mutable Inference: Architecting LLM Accelerators for Inference-Time Learning](https://doi.org/10.48550/arxiv.2611.18523)
<sub>2026-11-13 · Yimin Gao, Liangtao Dai, Melika Morsali 외 · arXiv (Cornell University)</sub>

> Long-context LLMs must retain growing histories, but full attention makes each new token increasingly expensive. Inference-time learning (ITL) offers another approach. The model keeps training on the context during inference, retaining what it learns in its weights. Recent work shows that ITL can match full-context attention quality while attending only to a recent fixed-size window. This bounds a

### ✅ [Perceptual-Centric Image Super-Resolution using Heterogeneous Processors on Mobile Devices](https://doi.org/10.1145/3636534.3690698)
<sub>2024-12-04 · Kai Huang, Xiangyu Yin, Tao Gu 외 · ACM Annual International Conference on Mobile Computing and Networking (MobiCom)</sub>

> Image super-resolution (SR) is widely used on mobile devices to enhance user experience. However, neural networks used for SR are computationally expensive, posing challenges for mobile devices with limited computing power. A viable solution is to use heterogeneous processors on mobile devices, especially the specialized hardware AI accelerators, for SR computations, but the reduced arithmetic pre

### ✅ [DSTAR: Accelerating Diffusion Transformers via Spatial and Temporal Redundancy Reduction](https://doi.org/10.48550/arxiv.2607.15846)
<sub>2026-07-17 · Chi Zhang, Jieru Zhao, Yu Feng 외 · arXiv (Cornell University)</sub>

> Diffusion Transformers (DiTs) have been widely used in many tasks, including image synthesis, video generation, and content editing. However, their multi-iteration inference process leads to performance inefficiency and high energy consumption. Existing acceleration methods primarily focus on reducing temporal redundancy between adjacent timesteps, but often overlook the specific features of DiTs.


## On-device AI accelerator

### 🆕 [One-Year Prediction of Vision-Threatening Diabetic Retinopathy Complications Using Multimodal Artificial Intelligence: A Multicenter Real-World Study](https://doi.org/10.21203/rs.3.rs-11433556/v1)
<sub>2026-11-18 · Mostafa EL HABIB DAHO, Philippe Zhang, Alireza Rezaei 외 · Research Square · 🚧 Virtual Short · Short</sub>

> Current diabetic retinopathy management relies primarily on contemporaneous severity grading and does not directly quantify the short-term risk of vision-threatening complications. We developed and internally evaluated image-based artificial intelligence models for one-year prediction of diabetic retinopathy severity, proliferative diabetic retinopathy (PDR) and center-involved diabetic macular ed

### 🆕 [SMBQ : An Efficient Stealing Multi‐Bucket Queue Scheduling Framework for Multicore Systems](https://doi.org/10.1002/cpe.71021)
<sub>2026-11-18 · Zhenhua Zhang, Wenwu Yu, Haofei Meng 외 · Concurrency and Computation Practice and Experience · 🚧 Independent source 제거 · Dependent source</sub>

> Ensuring rapid responses to high‐priority tasks, balancing workloads across threads, and efficiently utilizing computing resources are essential to improving the performance of resource‐constrained multicore platforms. However, existing priority scheduling methods face two major challenges. (1) Global ordering strategies can reduce redundant computation, but frequent cross‐thread synchronization c

### 🆕 [EdgeAgent: Orchestrating On-Device LLM inference for End-User Multi-Agent Systems on CPU-GPU Unified Memory Architectures](https://doi.org/10.1145/3845814.3850072)
<sub>2027-04-10 · Yuhai Long, Yuanxin Wei, Kai Wu 외 · International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS) · 🚧 Short Circuit Current · Rth 계산</sub>

> Emerging multi-agent LLMs demand privacy-preserving edge deployment, yet current inference systems struggle with these collaborative workflows. Specifically, the memory-bound decode phase causes severe bus contention on unified memory architectures (UMA), paralyzing naive CPU-GPU co-execution. Furthermore, speculative decoding in multi-agent workloads faces extreme variance in drafting difficulty,

### ✅ [Toward Edge General Intelligence With Agentic AI and Agentification: Concepts, Technologies, and Future Directions](https://doi.org/10.1109/comst.2026.3651702)
<sub>2026-01-01 · Ruichen Zhang, Guangyuan Liu, Yinqiu Liu 외 · IEEE Communications Surveys & Tutorials · 🚧 Independent source 제거 · Dependent source</sub>

> The rapid expansion of sixth-generation (6G) wireless networks and the Internet of Things (IoT) has catalyzed the evolution from centralized cloud intelligence towards decentralized edge general intelligence. However, traditional edge intelligence methods, characterized by static models and limited cognitive autonomy, fail to address the dynamic, heterogeneous, and resource-constrained scenarios i

### ✅ [Artificial intelligence in nursing: an integrative review of clinical and operational impacts](https://doi.org/10.3389/fdgth.2025.1552372)
<sub>2025-03-07 · Salwa Eweis Hassanein, Rabie Adel El Arab, Amany Ahmed Abdrbo 외 · Frontiers in Digital Health · 🚧 Operational Amplifier · Open-loop Operational Amplifier</sub>

> Background: Advances in digital technologies and artificial intelligence (AI) are reshaping healthcare delivery, with AI increasingly integrated into nursing practice. These innovations promise enhanced diagnostic precision, improved operational workflows, and more personalized patient care. However, the direct impact of AI on clinical outcomes, workflow efficiency, and nursing staff well-being re


## Neural rendering and NeRF accelerator

### 🆕 [Grounding Gaussian Splatting Geometry with Stochastic Solids](https://doi.org/10.1145/3829340.3842166)
<sub>2026-11-30 · Baowen Zhang, Chenxing Jiang, Heng Li 외 · SIGGRAPH Asia Conference Papers · 🚧 Open Circuit Voltage · Open Circuit</sub>

> Gaussian Splatting (GS) has demonstrated impressive quality and efficiency in novel view synthesis. However, shape extraction from Gaussian primitives remains an open problem. Due to inadequate geometry parameterization and approximation, existing shape reconstruction methods suffer from poor multi-view consistency and are sensitive to floaters. In this paper, we present a rigorous theoretical der

### 🆕 [A lightweight Gaussian-based framework for real-time facial expression enhancement in 3D avatar systems](https://doi.org/10.64820/aepjrr.32.1.7.122026)
<sub>2026-12-31 · Muhammad Shaheer, Safyan Jameel, Syed Farhad Shah Bukhari 외 · Journal of Robotics Research · 🚧 Virtual Short</sub>

> Facial expression modeling is a basic part of the contemporary 3D avatar systems as it plays an important role in emotional communication and engagement with the user and realism in the virtual environment. While there have been remarkable progress in neural rendering, Neural Radiance Field (NeRF) and Gaussian-based avatar representations have brought up impressive visual fidelity, the majority of

### 🆕 [OMEGA-Avatar: One-shot Modeling of 360° Gaussian Avatars](https://doi.org/10.1145/3829340.3842298)
<sub>2026-11-30 · 夏泽昊 Xia Zehao, Yiqun Wang, Zhengda Lu 외 · SIGGRAPH Asia Conference Papers · 🚧 Short Circuit Current</sub>

> Creating high-fidelity, animatable 3D avatars from a single image remains a formidable challenge. We identified three desirable attributes of avatar generation: 1) the method should create avatars from a single image in a one-shot setting without per-identity network optimization, 2) model a 360° full-head, and 3) produce animation-ready results. However, current works address only two of the thre

### ✅ [MoGe: Unlocking Accurate Monocular Geometry Estimation for Open-Domain Images with Optimal Training Supervision](https://doi.org/10.1109/cvpr52734.2025.00496)
<sub>2025-06-10 · Ruicheng Wang, Sicheng Xu, Cassie Dai 외 · IEEE Computer Society Conference on Computer Vision and Pattern Recognition/Proceedings - IEEE Computer Society Conference on Computer Vision and Pattern Recognition/Proceedings · 🚧 Open Circuit Voltage · Open Circuit</sub>

> We present MoGe, a powerful model for recovering 3D geometry from monocular open-domain images. Given a single image, our model directly predicts a 3D point map of the captured scene with an affine-invariant representation, which is agnostic to true global scale and shift. This new representation precludes ambiguous supervision in training and facilitates effective geometry learning. Furthermore, 

### ✅ [Gen3C: 3D-Informed World-Consistent Video Generation with Precise Camera Control](https://doi.org/10.1109/cvpr52734.2025.00574)
<sub>2025-06-10 · Xuanchi Ren, Tianchang Shen, Jiahui Huang 외 · IEEE Computer Society Conference on Computer Vision and Pattern Recognition/Proceedings - IEEE Computer Society Conference on Computer Vision and Pattern Recognition/Proceedings · 🚧 Infinite Input Resistance</sub>

> We present Gen3C, a generative video model with precise Camera Control and temporal 3D Consistency. Prior video models already generate realistic videos, but they tend to leverage little 3D information, leading to inconsistencies, such as objects popping in and out of existence. Camera control, if implemented at all, is imprecise, because camera parameters are mere inputs to the neural network whi


## Computing-in-memory and processing-in-memory

### 🆕 [BEHAVIORAL AND TEMPORAL FACTORS IN MALICIOUS-NODE DETECTION FOR RPL-BASED 6LoWPAN NETWORKS: A CONTROLLED SYNTHETIC STUDY](https://doi.org/10.17654/74101125)
<sub>2027-01-01 · KONE Kigninman Désiré, LOUKOU Kouadio Denis, Dozohoua Silue 외 · Far East Journal of Electronics and Communications · 🚧 Node Analysis · node voltage</sub>

> This controlled synthetic study examines how forwarding evidence, topology-oriented evidence, temporal context, and classifier choice influence malicious-node identification in RPL-oriented 6LoWPAN settings. Node behavior is characterized using inter-arrival time, packet forwarding ratio, rank inconsistency, and parent change rate. Thirty paired runs are conducted with 600 independent node profile

### 🆕 [Direct-Access-Enabled GPU Memory Offloading with Optimal Efficiency for LLM Inference](https://doi.org/10.1145/3845814.3850046)
<sub>2027-04-10 · Shouxu Lin, Zhiyuan Guo, Jiaxin Lin 외 · International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS) · 🚧 Independent source 제거 · Dependent source</sub>

> LLM inference is constrained by GPU memory capacity and bandwidth. Tiered memory architectures mitigate this by allowing the GPU to offload memory to the remote tier. However, existing memory offloading frameworks rely on prefetching data into local GPU HBM. This approach underutilizes system resources by introducing HBM contention, squandering memory capacity, and creating pipeline bubbles. We sh

### 🆕 [Evaluating Continual Learning Techniques in Edge AI for Real-Time Applications](https://doi.org/10.33425/3066-1226.1184)
<sub>2026-12-30 · Farheen Sultana, Mohd Zabih, Janardhan Golla 외 · Global Journal of Engineering Innovations and Interdisciplinary Research · 🚧 Independent source 제거 · Dependent source</sub>

> This research investigates the efficacy of various continual learning techniques—Elastic WeightConsolidation (EWC), Experience Replay, and Knowledge Distillation—within the framework of EdgeAI for real-time applications. Continual learning, crucial for adapting AI models to new data whilepreserving previously acquired knowledge, presents unique challenges when deployed on resource-constrained edge

### ✅ [NVILA: Efficient Frontier Visual Language Models](https://doi.org/10.1109/cvpr52734.2025.00390)
<sub>2025-06-10 · Zhijian Liu, Ligeng Zhu, Baifeng Shi 외 · IEEE Computer Society Conference on Computer Vision and Pattern Recognition/Proceedings - IEEE Computer Society Conference on Computer Vision and Pattern Recognition/Proceedings · 🚧 Open Circuit Voltage · Open Circuit</sub>

> Visual language models (VLMs) have made significant advances in accuracy in recent years. However, their efficiency has received much less attention. This paper introduces NVILA, a family of open VLMs designed to optimize both efficiency and accuracy. Building on top of VILA, we improve its model architecture by first scaling up the spatial and temporal resolutions, and then compressing visual tok

### ✅ [Reinforcement Learning via Self-Distillation](https://doi.org/10.48550/arxiv.2601.20802)
<sub>2026-01-28 · Jonas Hübotter, Frederike Lübeck, Lejs Behric 외 · arXiv (Cornell University) · 🚧 Short Circuit Current · Negative Feedback</sub>

> Large language models are increasingly post-trained with reinforcement learning in verifiable domains such as code and math. Yet, current methods for reinforcement learning with verifiable rewards (RLVR) learn only from a scalar outcome reward per attempt, creating a severe credit-assignment bottleneck. Many verifiable environments actually provide rich textual feedback, such as runtime errors or 

