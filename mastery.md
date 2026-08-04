---
title: "이해도 원장 (Mastery Ledger)"
kind: mastery
---

# 이해도 원장 — "진짜 공부했다"의 증거

> 개념마다 상태를 추적한다. **상태가 아니라 변화로** 기록한다.
> 상태: `미학습` → `암기`(답은 아는데 스스로 설명 못 함) → `설명가능`(스스로 유도·설명함).
> **`설명가능`은 AI의 반박을 통과하고, 증거(그 세션의 daily 링크)가 있을 때만.** 증거 없는 `설명가능`은 자기기만이다.
>
> ⚙️ 아래 표는 **자동 관리된다** — 세션에서 승급이 나오면 CI가 여기에 접어 넣는다.
> 손으로 고쳐도 되지만, `MASTERY-TABLE` 마커는 지우지 말 것(지우면 자동 갱신이 멈춘다).

<!-- MASTERY-TABLE:START -->
| 개념 | 상태 | 중요도 | 최근 검증일 | 증거(daily 세션) | 변화 메모(무엇이·왜 바뀌었나) |
|---|---|---|---|---|---|
| KCL | 암기 | H | 2026-08-02 | daily/2026-08-02-circuit-recovery-scan.md | 식과 계산은 기억하지만 전하 보존의 근거를 반대로 설명해 보완이 필요함 |
| KVL | 암기 | H | 2026-08-02 | daily/2026-08-02-circuit-recovery-scan.md | 전압 강하와 에너지 변환은 기억하지만 순에너지 변화 0까지 안정적으로 설명하는 검증이 더 필요함 |
| Thevenin Equivalent | 설명가능 | H | 2026-08-03 | daily/2026-08-03-thevenin-norton-equivalent.md | 단자 관점의 모델링 목적과 Vth, Rth의 역할을 자신의 말로 설명함 |
| Vth | 설명가능 | H | 2026-08-03 | daily/2026-08-03-thevenin-norton-equivalent.md | Open Circuit에서 I=0이고 내부 전압 강하가 없어 단자 전압이 Vth가 됨을 이해함 |
| Independent voltage source 제거 | 설명가능 | H | 2026-08-03 | daily/2026-08-03-thevenin-norton-equivalent.md | 0V 전압원이 Short와 동일한 이유를 설명함 |
| Independent current source 제거 | 설명가능 | H | 2026-08-03 | daily/2026-08-03-thevenin-norton-equivalent.md | 0A 전류원이 Open과 동일한 이유를 설명함 |
| Test Source | 설명가능 | H | 2026-08-03 | daily/2026-08-03-thevenin-norton-equivalent.md | Dependent source를 유지한 채 전압-전류 응답으로 Rth를 측정하는 이유를 설명함 |
| Norton Equivalent | 설명가능 | H | 2026-08-04 | daily/2026-08-04-thevenin-norton-review-2.md | Thevenin과의 관계 및 Open/Short의 목적을 자신의 말로 설명함 |
| Thevenin 알고리즘 | 설명가능 | H | 2026-08-04 | daily/2026-08-04-thevenin-norton-review-2.md | 풀이 순서를 스스로 수정하고 설명함 |
<!-- MASTERY-TABLE:END -->

## 읽는 법

- **암기**가 많다 = 답은 아는데 설명은 못 하는 상태. 그 개념부터 다시 설명해 보면 된다.
- **설명가능**이 늘어나는 것이 발전의 증거다. 개수보다 *무엇이* 올라갔는지를 본다.
- 같은 개념이 나중에 올라가면 새 줄로 쌓여 **변화**가 보인다(덮어쓰지 않는다).
