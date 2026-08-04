---
title: "Thevenin/Norton 원리 및 알고리즘 복원"
created: 2026-08-04
updated: 2026-08-04
tags: [learning]
source: "학습 세션 → Issue #8 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: gpt
source_issue: 8
---

# Thevenin/Norton 원리 및 알고리즘 복원

## 목표
- Thevenin/Norton Equivalent의 원리를 설명할 수 있다.
- Thevenin/Norton 문제 풀이 알고리즘을 복원한다.

## 예측 — 내가 먼저 답한 것
- Independent source를 먼저 제거하고 Rth를 구한 뒤 Vth를 구한다고 설명함.
- Norton은 전류원 + 병렬 저항 형태라는 것을 기억함.
- Thevenin을 만든 다음 Norton을 만드는 것인지 질문함.

## 오늘 직접 학습한 지식
1. Thevenin 문제 풀이 순서는 RL 제거(Open Circuit) → Vth 계산 → Independent Source 제거 → Rth 계산 → 등가회로 구성이다.
2. Vth는 Source가 살아있는 원래 회로에서 구해야 한다. Source를 먼저 제거하면 원래 회로의 특성을 잃는다.
3. Norton Equivalent는 Thevenin 이후에 만드는 것이 아니라 같은 회로를 표현하는 또 다른 등가 모델이다.
4. Norton은 Short Circuit Current를 이용해 전류원을 대표하며, Thevenin은 Open Circuit Voltage를 이용해 전압원을 대표한다.
5. Open Circuit은 회로가 만들어내는 단자 전압을 측정하기 위한 상태이고, Short Circuit은 회로가 공급할 수 있는 단자 전류를 측정하기 위한 상태이다.

## 교정 및 보완
- Source 제거는 Rth를 구할 때만 수행한다.
- Vth 계산 시에는 Independent Source를 제거하지 않는다.
- Thevenin과 Norton은 서로 변환 가능하지만 어느 한쪽을 반드시 먼저 구해야 하는 것은 아니다.

## 취약 영역
- 실제 시험 문제에서 계산 절차 검증
- Dependent Source가 포함된 Norton 문제

## 다음 복습 질문
1. Thevenin을 구하는 순서를 설명해보라.
2. Norton을 구하는 순서를 설명해보라.
3. 왜 Open Circuit과 Short Circuit을 각각 사용하는가?

## 개념 지도
### 전자회로
- Thevenin Equivalent ← Open Circuit Voltage, 등가 저항
- Norton Equivalent ← Short Circuit Current, 등가 저항
- Open Circuit Voltage ← Vth
- Short Circuit Current ← In
- Independent Source 제거 ← Rth 계산
