---
title: "Op-Amp 복원 시작"
created: 2026-08-05
updated: 2026-08-05
tags: [learning]
source: "학습 세션 → Issue #17 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: gpt
source_issue: 17
---

# Op-Amp 복원 시작

## 목표
- Op-Amp 복원을 시작한다.
- Virtual Short의 의미를 이해하고, Inverting / Non-Inverting Amplifier를 복원하기 위한 기반을 만든다.

## 예측 — 내가 먼저 답한 것
- "virtual short : 솔직히 기억안남 조금 어색함"
- "infinite Gain : Op-Amp 는 이론상 무한대로 증폭하기에, Vout = A(V+ - V-)이고 A가 무한대에 가까워서 V+ = V- 로 가정해서 회로를 이해하는 것"
- "Input Current = 0 : 이것역시 Op-Amp로 들어가는 current의 양은 0으로 두고 회로를 이해하는 것."
- "V+ = V- : 앞서 설명한 infinite gain에서 설명을 함. 무한대의 출력을 막기 위해서는 둘이 같아저야함."
- "Comparator : 비교자? 잘 기억안남."
- "Inverting / Non-inverting : 얘는 Op-Amp의 큰 두가지의 종류. 근데 정확하게 기억은 안남. 보면 바로 기억날듯."

## 오늘 직접 학습한 지식
1. Op-Amp의 출력은

   Vout = A(V+ - V-)

   로 표현된다.

2. Infinite Gain 자체 때문에 항상 V+ = V-가 되는 것이 아니라,
   Negative Feedback이 걸리고 Op-Amp가 정상 동작하는 경우에만
   입력 전압 차가 거의 0이 되도록 출력이 조절된다.

3. 따라서

   V+ ≈ V-

   는 Op-Amp의 기본 성질이 아니라
   Negative Feedback이 있는 경우에 사용할 수 있는 해석 규칙이다.

4. Input Current = 0은
   이상적인 Op-Amp의 입력 저항이 무한대라고 가정하기 때문에
   입력 단자로 전류가 흐르지 않는다는 의미이다.

5. Virtual Short는
   실제로 두 입력이 연결된 것이 아니라
   입력 전압만 거의 같게 유지되는 상태를 의미한다.

6. 진짜 Short와 Virtual Short의 차이

   - Short : 전압이 같고 전류도 흐를 수 있다.
   - Virtual Short : 전압은 거의 같지만 입력 전류는 0이다.

## 교정 및 보완
- "Infinite Gain이라서 항상 V+=V-"는 정확하지 않다.
- Negative Feedback이 존재해야 Virtual Short를 사용할 수 있다.
- Comparator에서는 Negative Feedback이 없기 때문에
  일반적으로 V+ = V-를 사용할 수 없다.
- Comparator는 다음 세션에서 복원하기로 한다.

## 퀴즈
- Q1 : 왜 Virtual Short는 Short가 아닌가?
  내 답 :
  아직 설명하지 못함.
  Input Current = 0과 연결해서 다시 복습 예정.

## 취약 영역
- Virtual Short를 자신의 말로 설명하기
- Negative Feedback의 역할
- Comparator
- Inverting Amplifier
- Non-Inverting Amplifier

## 다음 복습 질문
1. 왜 Virtual Short라고 부르는가?
2. Negative Feedback은 어떤 역할을 하는가?
3. Comparator에서는 왜 V+ = V-를 사용할 수 없는가?
4. Inverting Amplifier를 어떻게 유도하는가?
5. Non-Inverting Amplifier를 어떻게 유도하는가?

## 개념 지도

### 전자회로

Operational Amplifier ← Differential Amplifier

Infinite Gain ← Operational Amplifier

Input Current = 0 ← Infinite Input Resistance

Negative Feedback ← Operational Amplifier

Virtual Short ← Negative Feedback, Infinite Gain

Comparator ← Open-loop Operational Amplifier

Inverting Amplifier ← Virtual Short, Negative Feedback

Non-Inverting Amplifier ← Virtual Short, Negative Feedback

> ⚠️ 아래 헤딩은 수집기가 자동 보정했다 — 세션에 실제 기록이 없었다는 뜻이다.

## 현재 이해 수준
- (이번 세션 기록 없음)

## 미해결 질문
- (이번 세션 기록 없음)
