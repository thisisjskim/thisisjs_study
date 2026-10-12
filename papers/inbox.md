---
title: "논문 인박스 — 2026-10-12"
updated: 2026-10-12
kind: papers
---

# 📬 논문 인박스 — 2026-10-12

> 새 논문 **18편** — 🆕 신간(최근 14일, 최신순) + ✅ 검증(최근 2년, 인용순). 🚧 = 내 막힌 길목과 닿는 논문.
> 세션에서 *"이번 주 새 논문 같이 보자"* 라고 하면 러너가 여기서 골라 준다.
> 다 읽을 필요 없다 — **제목과 초록만 훑고 1편만 골라** 깊게 보는 편이 낫다.

> ⚠️ **분야가 고정되지 않은 주제 4개** — Yoo, Hoi-Jun, On-device AI accelerator, Neural rendering and NeRF accelerator, Computing-in-memory and processing-in-memory
> 이 주제들은 단어로만 검색된다. 약어가 겹치면 엉뚱한 분야의 논문이 섞인다(`HBM` → high bandwidth memory / human breast milk).
> 세션에서 러너에게 **"이 주제 분야 고정해줘"** 라고 하면, 이미 읽은 논문을 씨앗으로 삼아 분야를 잡아 준다 — 사람이 코드를 찾을 필요는 없다.

## Yoo, Hoi-Jun

### 🆕 [Which Expert Misses Are Worth Waiting For? Substitution and Caching for Mixture-of-Experts Inference on a Consumer GPU](https://doi.org/10.21203/rs.3.rs-11268552/v1)
<sub>2026-10-06 · ChaeWoo Son · Research Square · 🚧 Rth 계산</sub>

> _(초록이 공개돼 있지 않다 — 제목·저널로 판단하거나 원문을 열어 보자.)_

### ✅ [Panacea: Novel DNN Accelerator using Accuracy-Preserving Asymmetric Quantization and Energy-Saving Bit-Slice Sparsity](https://doi.org/10.1109/hpca61900.2025.00059)
<sub>2025-03-01 · Dongyun Kam, Myeongji Yun, Sunwoo Yoo 외 · Proceedings - International Symposium on High-Performance Computer Architecture/Proceedings</sub>

> Low bit-precisions and their bit-slice sparsity have recently been studied to accelerate general matrix-multiplications (GEMM) during large-scale deep neural network (DNN) inferences. While the conventional symmetric quantization facilitates low-resolution processing with bit-slice sparsity for both weight and activation, its accuracy loss caused by the activation’s asymmetric distributions cannot

### ✅ [RedFuser: An Automatic Operator Fusion Framework for Cascaded Reductions on AI Accelerators](https://doi.org/10.1145/3779212.3790209)
<sub>2026-03-10 · Xinsheng Tang, Yangcheng Li, Nan Wang 외 · ACM International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS)</sub>

> Operator fusion, as a key performance optimization technique in the deployment of AI models, significantly improves execution efficiency and has been widely adopted in modern AI compilers. However, for cascaded reduction operations involving multiple loops with inter-loop data dependencies, such as the safe softmax followed by GEMM within attention mechanisms, existing compilers lack effective aut


## On-device AI accelerator

### 🆕 [EdgePulse: A Runtime Observability Framework for Quantized Large Language Models on Consumer Edge Devices](https://doi.org/10.5281/zenodo.23248717)
<sub>2026-10-08 · Muhammad Assad Ullah · Zenodo (CERN European Organization for Nuclear Research) · 🚧 Open Circuit Voltage · Open Circuit</sub>

> On-device AI execution lacks unified runtime observability across mobile platforms. Existing tools focus on isolated model profiling or single-engine metrics and give no synchronized view of memory, thermal state, battery draw, and inference latency during real workloads. We present EdgePulse, an open-source runtime observability framework for on-device AI. EdgePulse captures structured InferenceT

### 🆕 [SATE AI: A Fault Injection and Reliability Engineering Framework for On-Device AI Models in Mobile Applications](https://doi.org/10.5281/zenodo.23250417)
<sub>2026-10-09 · Muhammad Assad Ullah · Zenodo (CERN European Organization for Nuclear Research) · 🚧 Independent source 제거 · Dependent source</sub>

> On-device artificial intelligence deployment in mobile applications confronts machine learning models with volatile hardware environments: unpredictable memory pressure, dynamic thermal constraints, and corrupted sensor inputs. Cloud-hosted systems enjoy active cooling, stable resource budgets, and established chaos engineering toolchains; mobile edge AI has none of these guarantees. Unhandled mod

### 🆕 [Multi‐Timescale In‐Sensor Reservoir Computing With Composition‐Engineered InSnO Optoelectronic Synaptic Transistors](https://doi.org/10.1002/adfm.78910)
<sub>2026-10-07 · Lan Ma, Xi Chen, Haoyang Shi 외 · Advanced Functional Materials · 🚧 Open Circuit Voltage · Open Circuit</sub>

> ABSTRACT Real‐time dynamic visual scenes often involve multiple objects moving at different speeds, requiring in‐sensor computing devices with dynamic responses matched to diverse motion timescales. Existing multi‐timescale reservoir systems generally rely on external biasing and closed‐loop feedback to modulate device time constants, increasing the complexity of peripheral control circuits and li

### ✅ [Integrating Artificial Intelligence and the Internet of Things in Cultural Heritage Preservation: A Systematic Review of Risk Management and Environmental Monitoring Strategies](https://doi.org/10.3390/buildings14123979)
<sub>2024-12-15 · Neeraparng Laohaviraphap, Tanut Waroonkun · Buildings</sub>

> Heritage buildings are increasingly vulnerable to environmental challenges like air pollution and climate change. Traditional preservation methods primarily rely on periodic inspections and manual interventions and struggle to address these evolving and dynamic threats. This systematic review analyzes how integrating Artificial Intelligence (AI) and Internet of Things (IoT) technologies can transf

### ✅ [Digital Twins Generated by Artificial Intelligence in Personalized Healthcare](https://doi.org/10.3390/app14209404)
<sub>2024-10-15 · M. Łukaniszyn, Łukasz Majka, Barbara Grochowicz 외 · Applied Sciences</sub>

> Digital society strategies in healthcare include the rapid development of digital twins (DTs) for patients and human organs in medical research and the use of artificial intelligence (AI) in clinical practice to develop effective treatments in a cheaper, quicker, and more effective manner. This is facilitated by the availability of large historical datasets from previous clinical trials and other 


## Neural rendering and NeRF accelerator

### 🆕 [DigiFish: A flexible open-source tool for animating realistic virtual fish and reconstructing visual fields from tracking data](https://doi.org/10.64898/2026.10.02.755892)
<sub>2026-10-06 · Katie Dunkley, Jolyon T. Troscianko, Anna Ahlberg 외 · bioRxiv (Cold Spring Harbor Laboratory) · 🚧 Virtual Short · Open Circuit Voltage</sub>

> Abstract For many animals, vision represents the primary sensory modality governing a vast diversity of behaviours. Creating ‘virtual twins’, or visually realistic digital reconstructions of real individuals interacting within their environments, offers a promising approach for understanding how visual information guides an animal’s decisions, behaviours, and interactions. Such systems enable the 

### 🆕 [Inaugural Editorial for Discover Computer Vision](https://doi.org/10.1007/s44584-026-00001-0)
<sub>2026-10-09 · Ziyou Wu, Xiaojun Qi · 🚧 Open Circuit Voltage · Open Circuit</sub>

> We are delighted to introduce Discover Computer Vision , a peer-reviewed, fully open access journal published by Springer Nature.

### 🆕 [Pano-to-3D: Multi-view consistent 3D indoor scene reconstruction from a single panorama image](https://doi.org/10.1016/j.cag.2026.104775)
<sub>2026-10-08 · Rong-Kai Xu, Lei Zhang · Computers & Graphics · 🚧 Independent source 제거 · Dependent source</sub>

> Single-view scene reconstruction presents significant challenges due to the limited viewpoint information. Panorama images, as a form of image representation with a 360° field of view (FoV), offer a richer source of information for scene reconstruction. Therefore, more and more work utilizes a single panorama image for scene reconstruction. However, existing methods for scene reconstruction from a

### ✅ [Vision-Language-Action Models for Robotics: A Review Towards Real-World Applications](https://doi.org/10.1109/access.2025.3609980)
<sub>2025-01-01 · Kento Kawaharazuka, Jihoon Oh, Jun Yamada 외 · IEEE Access</sub>

> Amid growing efforts to leverage advances in large language models (LLMs) and vision-language models (VLMs) for robotics, Vision-Language-Action (VLA) models have recently gained significant attention. By unifying vision, language, and action data at scale, which have traditionally been studied separately, VLA models aim to learn policies that generalise across diverse tasks, objects, embodiments,

### ✅ [A Multifaceted Vision of the Human-AI Collaboration: A Comprehensive Review](https://doi.org/10.1109/access.2025.3536095)
<sub>2025-01-01 · Maite Puerta-Beldarrain, Oihane Gómez–Carmona, Rubén Sánchez 외 · IEEE Access</sub>

> Human-AI collaboration has evolved into a complex, multidimensional paradigm shaped by research in various domains. Key areas such as human-in-the-loop systems, Interactive Machine Learning (IML), Hybrid Intelligence, and Human-Agent Interaction have significantly contributed to this development. However, these fields often lack cohesion, underscoring the need for a cohesive perspective to advance


## Computing-in-memory and processing-in-memory

### 🆕 [A lightweight attention-enhanced intrusion detection method for anomalous network traffic analysis](https://doi.org/10.1038/s41598-026-69052-x)
<sub>2026-10-09 · Xingguo Li, Peng Wu, Yuanyuan Xiong 외 · Scientific Reports · 🚧 Node Analysis · Independent source 제거</sub>

> Network intrusion detection in complex traffic environments requires a careful balance between detection performance and computational efficiency, particularly when models are intended for resource-constrained scenarios. Existing deep learning-based intrusion detection methods can achieve strong detection performance, but many of them rely on relatively complex architectures and may introduce cons

### 🆕 [Reproducible AES-128 Benchmarking and Security-Assessment Boundary for Resource-Constrained IoT Environments](https://doi.org/10.14445/23488379/ijeee-v13i9p105)
<sub>2026-10-08 · Manisha Ahirrao, Bageshree V. Pathak, Mrudul Dixit 외 · International Journal of Electrical and Electronics Engineering · 🚧 Node Analysis · Independent source 제거</sub>

> To meet the constraints of resource-constrained Internet of Things (IoT) devices, the encryption mechanism must provide confidentiality while adding little complexity and memory usage. This work presents a reproducible Advanced Encryption Standard (AES) -128 performance benchmarking and security boundary analysis for constrained IoT applications. Before any benchmarking, the AES-128 implementation

### 🆕 [Secure Boot and Firmware Update Framework for ARM Cortex-M Embedded IoT Devices](https://doi.org/10.31838/ece/03.02.01)
<sub>2026-10-16 · Lau Wei Cheng, Beh L. Wei · Progress in Electronics and Communication Engineering · 🚧 Independent source 제거 · Dependent source</sub>

> The paper presents a lightweight and well-impervious security framework suitable to ARM Cortex-M-based IOEs embedded devices, which will serve an important purpose of presenting secure boot and firmware update operations in resource-constrained systems. As IoT implementations and applications in sensitive parts of our life like healthcare, smart infrastructure, and industrial control systems incre

### ✅ [Industrial applications of large language models](https://doi.org/10.1038/s41598-025-98483-1)
<sub>2025-04-21 · Mubashar Raza, Zarmina Jahangir, Muhammad Bilal Riaz 외 · Scientific Reports</sub>

> Large language models (LLMs) are artificial intelligence (AI) based computational models designed to understand and generate human like text. With billions of training parameters, LLMs excel in identifying intricate language patterns, enabling remarkable performance across a variety of natural language processing (NLP) tasks. After the introduction of transformer architectures, they are impacting 

### ✅ [Tiny Machine Learning and On-Device Inference: A Survey of Applications, Challenges, and Future Directions](https://doi.org/10.3390/s25103191)
<sub>2025-05-19 · Soroush Heydari, Qusay H. Mahmoud · Sensors</sub>

> The growth in artificial intelligence and its applications has led to increased data processing and inference requirements. Traditional cloud-based inference solutions are often used but may prove inadequate for applications requiring near-instantaneous response times. This review examines Tiny Machine Learning, also known as TinyML, as an alternative to cloud-based inference. The review focuses o

