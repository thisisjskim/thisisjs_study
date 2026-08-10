---
title: "논문 인박스 — 2026-08-10"
updated: 2026-08-10
kind: papers
---

# 📬 논문 인박스 — 2026-08-10

> 새 논문 **3편** — 🆕 신간(최근 14일, 최신순) + ✅ 검증(최근 2년, 인용순). 🚧 = 내 막힌 길목과 닿는 논문.
> 세션에서 *"이번 주 새 논문 같이 보자"* 라고 하면 러너가 여기서 골라 준다.
> 다 읽을 필요 없다 — **제목과 초록만 훑고 1편만 골라** 깊게 보는 편이 낫다.

> ⚠️ **조회 실패 3개 주제** — On-device AI accelerator, Neural rendering and NeRF accelerator, Computing-in-memory and processing-in-memory
> 새 논문이 없는 것이 아니라 **가져오지 못한** 것이다. Actions 로그를 보고
> `paper-scan → Run workflow`로 다시 돌리면 된다.

> ⚠️ **분야가 고정되지 않은 주제 4개** — Yoo, Hoi-Jun, On-device AI accelerator, Neural rendering and NeRF accelerator, Computing-in-memory and processing-in-memory
> 이 주제들은 단어로만 검색된다. 약어가 겹치면 엉뚱한 분야의 논문이 섞인다(`HBM` → high bandwidth memory / human breast milk).
> 세션에서 러너에게 **"이 주제 분야 고정해줘"** 라고 하면, 이미 읽은 논문을 씨앗으로 삼아 분야를 잡아 준다 — 사람이 코드를 찾을 필요는 없다.

## Yoo, Hoi-Jun

### 🆕 [Unified Lookup-Table Inference with Signed-Digit K/V Caches for Ternary LLMs](https://arxiv.org/abs/2608.03229)
<sub>2026-08-04 · Ziang Duan, Jiajun Wu, Zetian Chen 외 · arXiv (Cornell University)</sub>

> Ternary LLMs make their weight-dominated projections compact and efficient, but attention remains a mismatch: its K/V cache is created online and is typically processed by a separate higher-precision engine. Compressing this cache alone does not resolve the mismatch. To execute attention with the same lookup-table machinery as ternary projections, values accumulated in one reduction must retain a 

### ✅ [GCC: A 3DGS Inference Architecture with Gaussian-Wise and Cross-Stage Conditional Processing](https://doi.org/10.1145/3725843.3756072)
<sub>2025-10-17 · Minnan Pei, Gang Li, Junwen Si 외 · 🚧 Independent source 제거 · Dependent source</sub>

> 3D Gaussian Splatting (3DGS) has emerged as a leading neural rendering technique for high-fidelity view synthesis, prompting the development of dedicated 3DGS accelerators for resource-constrained platforms.The conventional decoupled preprocessing-rendering dataflow in existing accelerators has two major limitations: 1) a

### ✅ [iDSE: Navigating Design Space Exploration in High-Level Synthesis Using LLMs](https://doi.org/10.48550/arxiv.2505.22086)
<sub>2025-05-28 · Rui Li, Xiong, Jia, Xi Wang 외 · arXiv (Cornell University) · 🚧 Open Circuit Voltage · Open Circuit</sub>

> High-Level Synthesis (HLS) serves as an agile hardware development tool that streamlines the circuit design by abstracting the register transfer level into behavioral descriptions, while allowing designers to customize the generated microarchitectures through optimization directives. However, the combinatorial explosion of possible directive configurations yields an intractable design space. Tradi

