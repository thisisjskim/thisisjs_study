---
title: "논문 인박스 — 2026-10-05"
updated: 2026-10-05
kind: papers
---

# 📬 논문 인박스 — 2026-10-05

> 새 논문 **18편** — 🆕 신간(최근 14일, 최신순) + ✅ 검증(최근 2년, 인용순). 🚧 = 내 막힌 길목과 닿는 논문.
> 세션에서 *"이번 주 새 논문 같이 보자"* 라고 하면 러너가 여기서 골라 준다.
> 다 읽을 필요 없다 — **제목과 초록만 훑고 1편만 골라** 깊게 보는 편이 낫다.

> ⚠️ **분야가 고정되지 않은 주제 4개** — Yoo, Hoi-Jun, On-device AI accelerator, Neural rendering and NeRF accelerator, Computing-in-memory and processing-in-memory
> 이 주제들은 단어로만 검색된다. 약어가 겹치면 엉뚱한 분야의 논문이 섞인다(`HBM` → high bandwidth memory / human breast milk).
> 세션에서 러너에게 **"이 주제 분야 고정해줘"** 라고 하면, 이미 읽은 논문을 씨앗으로 삼아 분야를 잡아 준다 — 사람이 코드를 찾을 필요는 없다.

## Yoo, Hoi-Jun

### 🆕 [IMC-CLINIC: Coupled Loss-Informed Newton Iterations for Clipping in Analog In-Memory Computing](https://doi.org/10.48550/arxiv.2609.35586)
<sub>2026-09-28 · Yung-Chin Chen, Chia‐Yu Chen, Dr. Naveen Verma 외 · arXiv (Cornell University) · 🚧 Independent source 제거 · Dependent source</sub>

> Analog in-memory computing (IMC) offers a promising path toward energy-efficient large language model (LLM) inference by executing matrix multiplications (MatMul) directly within memory arrays in the analog domain. Its efficiency, however, comes with an additional source of error: limited-precision analog-to-digital converters (ADCs) quantize accumulated analog partial sums, introducing output-sid

### ✅ [Design and Development of a Neuromorphic Silicon Suite: PVT Sensing, Stochastic LIF Inference, On-Chip STDP Learning, and Crossbar Programming](https://doi.org/10.48550/arxiv.2606.22635)
<sub>2026-06-21 · Poornima Kumaresan, Santhosh Sivasubramani · arXiv (Cornell University) · 🚧 node voltage · Open Circuit Voltage</sub>

> Edge neuromorphic systems need compact, configurable hardware that combines probabilistic inference, local learning, and an interface to emerging analogue memory. We present four interface-compatible digital IP blocks implemented as standard-cell CMOS on the SkyWater 130 nm process: a process, voltage and temperature (PVT) sensor built from five selectable ring oscillators that also provides a jit

### ✅ [Fine-Grained Fusion: The Missing Piece in Area-Efficient State Space Model Acceleration](https://doi.org/10.1109/pact65351.2025.00034)
<sub>2025-11-03 · Robin Geens, Arne Symons, Marian Verhelst 외 · 🚧 Node Analysis</sub>

> State Space Models (SSMs) offer a promising alternative to transformers for long-sequence processing. However, their efficiency remains hindered by memory-bound operations, particularly in the prefill stage. While MARCA, a recent first effort to accelerate SSMs through a dedicated hardware accelerator, achieves a great speedup over high-end GPUs, an analysis of the broader accelerator design space


## On-device AI accelerator

### 🆕 [Smart Port Technologies: A Scoping Review](https://doi.org/10.65154/ijmst.57)
<sub>2026-09-30 · Tran Xuan The, Thomas Do, Quoc Dong Hoang 외 · International Journal of Marine Science and Technology · 🚧 Node Analysis · node voltage</sub>

> The maritime industry is undergoing a profound digital transformation, with smart ports emerging as critical nodes in global supply chains. This comprehensive literature review synthesizes current research on key enabling technologies for smart ports, including Digital Twins, Blockchain, Artificial Intelligence, Internet of Things (IoT), Computer Vision, Unmanned Aerial Vehicles (UAVs), automation

### 🆕 [Barriers to the Adoption of Industry 4.0 Technologies in the Digital Agri-Food Supply Chain](https://doi.org/10.33889/ijmems.2026.11.5.094)
<sub>2026-09-29 · Mansi Singh, Viket Saurabh, Sagar Bharti 외 · International Journal of Mathematical Engineering and Management Sciences · 🚧 Independent source 제거 · Dependent source</sub>

> Food waste in the agricultural sector remains a critical challenge with far-reaching impacts for food security and resource efficiency. In response, digitalization has increasingly been integrated into the Agri-Food Supply Chain (AFSC) to ease these losses. However, before effective digital solutions can be implemented, it is essential to identify and cognize the barriers within the digital AFSC. 

### 🆕 [Robust Edge Trade-off Index (RETI): A multi-criteria framework for reliable and resource-aware deep learning model selection](https://doi.org/10.1016/j.array.2026.101280)
<sub>2026-09-26 · Oluwaseun O. Martins, Christiaan Coenrad Oosthuizen, Dawood Desai 외 · Array · 🚧 Independent source 제거 · Dependent source</sub>

> The deployment of deep learning models on resource-constrained edge platforms requires model-selection strategies that account for predictive accuracy, reliability, robustness, and computational cost simultaneously. Conventional evaluation commonly treats these criteria independently, making the selection of an appropriate model difficult when candidate architectures exhibit conflicting performanc

### ✅ [Predetermined Change Control Plans: Guiding Principles for Advancing Safe, Effective, and High-Quality AI-ML Technologies](https://doi.org/10.2196/76854)
<sub>2025-10-31 · Eduardo Carvalho, Miguel Mascarenhas, Francisca Pinheiro 외 · JMIR AI · 🚧 Short Circuit Current</sub>

> Unlabelled: The adaptive nature of artificial intelligence (AI), with its ability to improve performance through continuous learning, offers substantial benefits across various sectors. However, current regulatory frameworks are not intended to accommodate this adaptive nature, and they have prolonged approval timelines, sometimes exceeding one year for some AI-enabled devices. This creates signif

### ✅ [Artificial intelligence advances in anomaly detection for telecom networks](https://doi.org/10.1007/s10462-025-11108-x)
<sub>2025-01-25 · Enerst Edozie, Aliyu Nuhu Shuaibu, Bashir Olaniyi Sadiq 외 · Artificial Intelligence Review</sub>

> Telecommunication networks are becoming increasingly dynamic and complex due to the massive amounts of data they process. As a result, detecting abnormal events within these networks is essential for maintaining security and ensuring seamless operation. Traditional methods of anomaly detection, which rely on rule-based systems, are no longer effective in today’s fast-evolving telecom landscape. Th


## Neural rendering and NeRF accelerator

### 🆕 [Algorithmic Storage: The Algorithmic disk on the Footprint–Compute–Horizon Triangle](https://doi.org/10.59256/ijsreat.20260605004)
<sub>2026-09-29 · Patil Milind k · International Journal Of Scientific Research In Engineering & Technology · 🚧 Independent source 제거 · Dependent source</sub>

> Algorithmic Storage is a paradigm in which data is regenerated rather than retained: a spatial cost, storage, is converted into a temporal one, regeneration time. Its device, the Algorithmic Disk, holds only shared generator engines and one small Seed per object, and regenerates any object on demand, bit-exactly, by running an engine—the Algorithmic NET—forward from the Seed. The three resources a

### 🆕 [BridgeDiff: A two-stage conditional diffusion model for bridge point clouds completion](https://doi.org/10.1016/j.aei.2026.105314)
<sub>2026-09-29 · Yunping Fang, Mohammad Reza Salami, Stergios-Aristoteles Mitoulis 외 · Advanced Engineering Informatics · 🚧 Short Circuit Current · Rth 계산</sub>

> Scanned point clouds of civil infrastructure are often incomplete due to scanning limitations, making point cloud completion an essential task for Scan-to-BIM workflows. The complex geometries of structures further challenge point cloud completion methods. Currently, most completion models focus solely on synthetic small object datasets or autonomous driving scenarios. In this paper, going beyond 

### 🆕 [A Survey of Robotic Navigation and Manipulation with Physics Simulators in the Era of Embodied AI](https://doi.org/10.1145/3856802)
<sub>2026-10-03 · Liang Wei Wong, Xueyang Kang, Kaixin Bai 외 · ACM Computing Surveys</sub>

> Navigation and manipulation are core capabilities in Embodied AI, but training agents to perform them directly in the real world is costly, time-consuming, and unsafe. Therefore, sim-to-real transfer has emerged as a key approach, yet the sim-to-real gap persists. This survey examines how physics simulators address this gap by analyzing properties that have received limited attention in prior surv

### ✅ [Toward a Ludic Architecture. The Space of Play and Games](https://doi.org/10.1184/r1/6686981)
<sub>2024-10-28 · Steffen P. Walz · Figshare</sub>

> Toward a Ludic Architecture is a pioneering publication, architecturally framing play and games as human practices in and of space. Filling the gap in literature, Steffen P. Walz considers game design theory and practice alongside architectural theory and practice, asking: how are play and games architected? What kind of architecture do they produce and in what way does architecture program play a

### ✅ [A Survey on 3D Gaussian Splatting](https://doi.org/10.1145/3807511)
<sub>2026-04-09 · Guikun Chen, Wenguan Wang · ACM Computing Surveys</sub>

> 3D Gaussian splatting (GS) has emerged as a transformative technique in radiance fields. Unlike mainstream implicit neural models, 3D GS uses millions of learnable 3D Gaussians for an explicit scene representation. Paired with a differentiable rendering algorithm, this approach achieves real-time rendering and unprecedented editability, making it a potential game-changer for 3D reconstruction and 


## Computing-in-memory and processing-in-memory

### 🆕 [Intelligent Fault Diagnosis and Root-Cause Analytics for Renewable Power Converters Using Machine Learning Techniques Effectively](https://doi.org/10.7753/ijsea1510.1004)
<sub>2026-10-01 · Ravanbakhsh Leikh · International Journal of Science and Engineering Applications · 🚧 node voltage · Open Circuit Voltage</sub>

> The accelerating integration of renewable energy resources into modern power systems has increased reliance on power electronic converters for efficient energy conversion, grid synchronization, voltage regulation, and power-quality management.However, converters deployed in photovoltaic, wind, and energy-storage systems operate under variable loading, switching stresses, thermal cycling, environme

### 🆕 [In‐Memory Computing Using Memristors](https://doi.org/10.1002/9781394390274.ch15)
<sub>2026-10-02 · G. H. V. S. M. Soma Sai, P. Ramakrishna, S. Kala 외 · 🚧 Open Circuit Voltage · Open Circuit</sub>

> Memristors represent the fourth fundamental circuit element that is actively transforming in-memory computing (IMC) through solution of traditional von Neumann architecture issues. The arrangement of processing units and memory in conventional systems becomes obsolete because memristors allow computation to take place directly within memory arrays. Data transfers occur less frequently because of t

### 🆕 [Strategy dependent recruitment of distributed cortical circuits during spatial navigation](https://doi.org/10.1523/jneurosci.0674-24.2026)
<sub>2026-10-01 · Daniel A. Surinach, Mathew L. Rynes, Kapil Saxena 외 · Journal of Neuroscience · 🚧 Open Circuit Voltage · Open Circuit</sub>

> Spatial navigation involves neural computations in distributed regions of the brain. Little is known about how activity across cortical regions is coordinated when animals navigate novel spatial environments or how that coordination changes as environments become familiar. We recorded mesoscale calcium (Ca2+) dynamics across large swathes of the dorsal cortex in male mice solving the Barnes maze, 

### ✅ [Cloud–edge–device collaborative computing in smart agriculture: architectures, applications, and future perspectives](https://doi.org/10.3389/fpls.2025.1668545)
<sub>2025-10-14 · Pengpeng Yu, Fei Teng, Wenhui Zhu 외 · Frontiers in Plant Science · 🚧 Independent source 제거 · Dependent source</sub>

> Smart agriculture is rapidly evolving in response to growing global demands for food security and sustainable resource management. Cloud-edge-device collaborative computing has emerged as a transformative paradigm, addressing the limitations of traditional centralized architectures by enabling distributed intelligence, real-time processing, and adaptive decision-making. This review provides a comp

### ✅ [A Survey of Security in UAVs and FANETs: Issues, Threats, Analysis of Attacks, and Solutions](https://doi.org/10.1109/comst.2024.3515051)
<sub>2024-12-11 · Özlem Ceviz, Sevil Şen, Pinar Sadioglu 외 · IEEE Communications Surveys & Tutorials · 🚧 Node Analysis</sub>

> Thanks to the rapidly developing technology, unmanned aerial vehicles (UAVs) are able to complete a number of tasks in cooperation with each other without need for human intervention. In recent years, UAVs, which are widely utilized in military missions, have begun to be deployed in civilian applications and mostly for commercial purposes. With their growing numbers and range of applications, UAVs

