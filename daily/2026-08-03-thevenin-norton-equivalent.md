---
title: "테브난 등가회로 원리 복원"
created: 2026-08-03
updated: 2026-08-03
tags: [learning]
source: "학습 세션 → Issue #7 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: gpt
source_issue: 7
---

# 테브난 등가회로 원리 복원

## 목표
- Thevenin Equivalent의 목적, Open Circuit Voltage, 등가 저항, 독립·종속 전원 처리 원리를 이해한다.
- Norton Equivalent와의 연결을 위한 기반을 만든다.

## 예측 — 내가 먼저 답한 것
- "Thevenin Equivalent 이름이 기억나. 대충 그 원리도 알고 있어. 병렬도 연결되어 있는 current source를 전압과 저항의 직렬로 변환시켜서 회로의 이해를 돕는 방법이지. 그런데 내가 Thevenin Equivalent을 이용하여 문제를 푸는 과정이 솔직히 기억이 잘 안나. dependence source, independence source가 섞여 있거나, 이 중 하나만 있거나, 이런 과정마다 Thevenin Equivalent 를 사용하는 방법이 다 달랐던 것 같은데, 이 내용은 기억이 잘 안남. 같은 맥락으로 Norton 도 마찬가지"
- "왜냐하면 복잡한 회로 구성을 단순화 하는 것은 매우 어려운 일이고, 우리가 진짜 중요한 것은 결국 특정 '저항'에 얼마큼의 전류 or 전압이 흐르는지가 궁금하기 때문에, 그 관점에서 다른 source나 저항 등을 단순화하는거야."
- "그러게 잘 모르겠네,, 테브날의 목적이, 어떤 회로가 있고 그 주어진 회로에 RL이라는 부하를 첨가했을 때 그 RL(부하)에 걸리는 전류 전압을 측정하는 것이 목적이야? 그런 논리대로 하는거라면, RL 이전의 상태에서의 전압차를 측정한 후 RL을 달았을 때 기존 회로에서 어떤식으로 반응하는지 확인하는 것으로 이해하면 되나? 내가 말해도 조금 이상하네. 명확하게 알려줘. 내가 어떤 부분을 잘못이해하고 있는지도"
- "외부 tool을 이용해서 회로 그림을 잘 그려줘. 지금 너무 회로 그림을 이해하기 어려워"
- "오케이 다시 설명해줄게, Vth를 RL을 떼어낸 상태에서 측정하는 이유는, 우리는 RL의 변화에 따라서 RL에 흐르는 전압강하나 전류를 구하고 싶은거야. 그러기 위해서는 RL이 포함되지 않은(떼어낸 상태)의 회로를 먼저 분석해야 해. 그래서 RL이 포함되지 않은 상태에서의 Vth를 측정한 후, 이후 여기에 우리가 궁금한 RL이 부착되었을 때 어떤식으로 변하는지를 측정하는 거야. 나의 설명이 어때"
- "전압이 떨어진 이유는, 핸드폰 내부 저항으로 인하여 내부 전압강하가 이루어졌기 때문이지. Vth는 핸드폰이 연결되지 이전의 전압이고, 내부 저항이 추가되면 언제든지 바꿀 수 있어"
- "그 어떤 저항을 연결해도, 그 저항을 연결하기 이전 회로에서의 전압차를 측정하여 그 전압차(Vth)의 특성을 지닌 회로를 분석하기 위해서지. 그 회로에 RL이 붙었을 때 기존 Vth와의 관계를 유도하여 회로를 풀어나갈꺼야"
- "복잡한 회로에서 만들어내는 전체 전압, 저항을 계산했기 때문에 RL이 왔을 때 Vth와 Rth값을 이용하여 RL에 얼마큼의 전류와 전압강하가 일어나는지 알 수 있어"
- "0V 전압원은 사실상 전압강하가 일어나지 않고, 이는 저항이 없는 전류의 흐름으로 이해할 수 있기 때문에 단순한 도선으로 생각하여 short라고 판단할 수 있기 때문이야"
- "0A 전류원은 전류가 흐르지 않는 상태이기 때문에, 이는 open과 다름이 없지"
- "얘는 0V로 바꿀 수 없어. 왜냐하면 Vx에 따라 V가 변화하기 때문이야. 따라서 Vx를 함께 고려해줘야해"
- "dependent source가 있을 때, 얘를 들면 V = 2Vx 일때, 우리는 Vx의 값을 몰라. 회로가 복잡하기 때문이지. 그래서 source를 함부로 끌 수 없을 뿐더러, Vx를 0으로 둘 수도 없어. 따라서 test current나 test voltage를 가해줌으로써 이 회로에서 일어나는 상호작용, 즉 전류와 전압의 비를 통해서 저항을 측정하는거야."

## 오늘 직접 학습한 지식
1. Thevenin Equivalent는 복잡한 회로 전체를 그대로 단순화하는 것이 아니라, RL이 연결될 두 단자에서 본 회로의 특성을 Vth와 Rth로 모델링하는 방법이다.
2. Vth는 RL을 떼어낸 Open Circuit 상태의 단자 전압이다. Open Circuit에서는 전류가 0이므로 Rth에서 전압 강하가 없고, 단자 전압이 그대로 Vth가 된다.
3. Vth와 Rth를 알면 RL이 바뀌어도 직렬회로의 전류와 전압분배를 이용해 RL의 전류와 전압을 계산할 수 있다.
4. Independent voltage source를 0V로 만들면 양단 전위차가 0이 되어 Short와 동일하게 동작한다.
5. Independent current source를 0A로 만들면 해당 가지에 전류가 흐르지 않아 Open과 동일하게 동작한다.
6. Dependent source는 회로 내부 변수 Vx나 Ix에 따라 값이 정해지므로 임의로 끌 수 없다.
7. Dependent source가 있는 회로에서는 test voltage 또는 test current를 가하고, 회로의 응답에서 전압과 전류의 비를 구해 Rth를 측정한다.

## 교정 및 보완
- 병렬 current source를 직렬 voltage source와 저항으로 바꾸는 것은 Source Transformation이며, Thevenin Equivalent와 관련은 있지만 같은 개념은 아니다.
- Thevenin Equivalent의 목적은 특정 RL 하나만 푸는 것이 아니라, RL이 연결될 단자에서 본 원래 회로의 특성을 Vth와 Rth로 모델링하는 것이다.
- "복잡한 회로의 전체 전압과 전체 저항"보다는 "RL이 연결될 단자에서 본 등가 전압과 등가 저항"이라고 표현해야 정확하다.
- 휴대폰 연결 후 전압이 감소하는 Thevenin 예시에서는 휴대폰 내부저항이 아니라 전원 쪽의 Rth에서 전압 강하가 생긴다고 봐야 한다.
- 0V 전압원이 Short인 핵심 이유는 저항이 0이라고 가정해서가 아니라, 양단 전위차를 항상 0V로 강제해 이상적인 도선과 구별되지 않기 때문이다.
- Norton Equivalent의 계산 절차와 Short Circuit Current는 아직 직접 검증하지 않았다.

## 퀴즈
- Q1: 왜 Vth를 Open Circuit에서 구하는가? / 내 답: "그 어떤 저항을 연결해도, 그 저항을 연결하기 이전 회로에서의 전압차를 측정하여 그 전압차(Vth)의 특성을 지닌 회로를 분석하기 위해서지. 그 회로에 RL이 붙었을 때 기존 Vth와의 관계를 유도하여 회로를 풀어나갈꺼야" / 채점: 방향은 맞음. Open Circuit에서 I=0이라 Rth의 전압 강하가 0이고 단자 전압이 Vth가 된다는 물리적 이유를 보완함.
- Q2: 왜 0V 전압원은 Short인가? / 내 답: "0V 전압원은 사실상 전압강하가 일어나지 않고, 이는 저항이 없는 전류의 흐름으로 이해할 수 있기 때문에 단순한 도선으로 생각하여 short라고 판단할 수 있기 때문이야" / 채점: 핵심 정답. 양단 전위차를 항상 0V로 강제한다는 표현으로 보완함.
- Q3: 왜 0A 전류원은 Open인가? / 내 답: "0A 전류원은 전류가 흐르지 않는 상태이기 때문에, 이는 open과 다름이 없지" / 채점: 정답.
- Q4: 왜 Dependent source가 있으면 Test Source를 사용하는가? / 내 답: "dependent source가 있을 때, 얘를 들면 V = 2Vx 일때, 우리는 Vx의 값을 몰라. 회로가 복잡하기 때문이지. 그래서 source를 함부로 끌 수 없을 뿐더러, Vx를 0으로 둘 수도 없어. 따라서 test current나 test voltage를 가해줌으로써 이 회로에서 일어나는 상호작용, 즉 전류와 전압의 비를 통해서 저항을 측정하는거야." / 채점: 핵심 원리 설명 가능.

## 취약 영역
- 실제 회로에서 Vth와 Rth를 계산하는 문제 풀이 순서
- Independent source만 있는 회로와 Dependent source가 포함된 회로의 적용
- Norton Equivalent의 Short Circuit Current와 Thevenin-Norton 변환
- Source Transformation과 Thevenin/Norton Equivalent의 구분

## 다음 복습 질문
1. 왜 Open Circuit에서 측정한 단자 전압이 Vth와 같은가?
2. Independent source만 있는 회로에서 Rth를 구하는 절차는 무엇인가?
3. Dependent source가 포함된 회로에서 Test Source로 Rth를 구하는 절차는 무엇인가?
4. Norton current는 어떤 상태에서 구하며, Vth 및 Rth와 어떤 관계인가?

## 개념 지도
### 회로 등가화
- Thevenin Equivalent ← 단자 관점, Open Circuit Voltage, 등가 저항
- Vth ← Open Circuit, 단자 전압
- Rth ← Independent source 제거, Test Source
- Independent voltage source 제거 ← 0V 전압원, Short
- Independent current source 제거 ← 0A 전류원, Open
- Test Source ← Dependent source, 전압-전류 응답
- Norton Equivalent ← Thevenin Equivalent, Short Circuit Current
- Source Transformation ← 전압원-전류원 변환
