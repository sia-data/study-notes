# A/B Test Experiment Log Template 

## Overview

This template helps marketing, product, and UX teams **plan, document, and reflect on A/B tests** with a structured and repeatable format. Keeping a shared, detailed log helps ensure experiment quality, team alignment, and learnings accumulation.

---

## 1. Why You Need an Experiment Log

* Institutional memory: Track what was tested and why
* Replicability: Reuse validated experiments or avoid failed ones
* Strategic alignment: Link to OKRs and broader goals
* Continuous improvement: Capture learnings regardless of result

---

## 2. Experiment Log Template Structure

| Field                  | Description                                                             |
| ---------------------- | ----------------------------------------------------------------------- |
| Experiment ID          | Unique identifier (e.g., AB-2024-04-001)                                |
| Experiment Name        | Clear title (e.g., "Homepage CTA Redesign")                             |
| Objective              | What are you trying to improve? (e.g., Signup Rate)                     |
| Hypothesis             | If X, then Y... (e.g., If we simplify the CTA, users will sign up more) |
| Primary Metric         | Success criteria (e.g., Signup Conversion Rate)                         |
| Secondary Metrics      | Supporting indicators (e.g., Bounce Rate, Time on Page)                 |
| Guardrail Metrics      | Ensure no harm (e.g., Error rate, Page load time)                       |
| Target Audience        | Who is being tested? (e.g., new users, mobile only)                     |
| Sample Size & Duration | Minimum users and time required for significance                        |
| Start & End Date       | When was it live?                                                       |
| Variant Details        | What was changed in each version (A vs B)?                              |
| Tools Used             | GA4, Amplitude, Mixpanel, Optimizely, VWO, etc.                         |
| Statistical Method     | t-test, chi-square, Bayesian, etc.                                      |
| Result Summary         | Did the variant win? Was it significant?                                |
| p-Value / CI           | Statistical significance report                                         |
| Action Taken           | What was implemented based on the result?                               |
| Learnings              | What should we apply or avoid next time?                                |

> 💡 TIP: Store this template in a Notion/Confluence/Google Sheet and link it to dashboards and OKRs.

---

## 3. Best Practices

* Define one primary metric per test (avoid multiple KPIs)
* Test one change at a time unless using multivariate setup
* Document hypothesis **before** test starts
* Always track guardrail metrics to avoid negative side effects
* Visualize results and effect size, not just p-values

---

# A/B 테스트 실험 로그 템플릿 (Experiment Log Template)

## 개요

이 템플릿은 마케팅/제품/UX팀이 **A/B 테스트를 체계적으로 설계, 실행, 회고**할 수 있도록 돕는 실무용 문서입니다. 기록을 남기면 실험 품질이 향상되고, 팀 내 학습이 누적되며, 전략적 의사결정이 쉬워집니다.

---

## 1. 왜 실험 로그가 필요한가?

* 조직적 학습 자산 축적 (무엇을 왜 테스트했는지 기억 가능)
* 재현성 확보 (성공 실험은 재활용, 실패는 피할 수 있음)
* 전략 정렬 (OKR과 연계된 실험 우선순위 설정)
* 성과 회고 기반 개선 (실패도 다음 실험에 기여할 수 있음)

---

## 2. 실험 기록 템플릿 항목

| 항목             | 설명                                    |
| -------------- | ------------------------------------- |
| 실험 ID          | 고유 실험번호 (예: AB-2024-04-001)           |
| 실험명            | 명확한 제목 (예: ‘홈페이지 CTA 문구 변경 실험’)       |
| 목표             | 실험을 통해 개선하려는 지표 (예: 가입 전환율)           |
| 가설             | X를 하면 Y가 증가할 것이다 (예: CTA 단순화 시 가입 증가) |
| 주요 지표          | 실험의 핵심 성공 기준 (예: Signup 전환율)          |
| 보조 지표          | 참고 지표 (예: 이탈률, 페이지 체류시간 등)            |
| 가드레일 지표        | 부정적 효과 방지를 위한 체크 (예: 로딩 속도, 에러율)      |
| 대상 그룹          | 테스트 대상 유저 (예: 신규 사용자, 모바일 유저 등)       |
| 샘플 크기 및 기간     | 통계적 유의성을 확보할 최소 사용자 수 및 기간            |
| 실험 기간          | 시작일 / 종료일                             |
| 버전 설명          | A/B 각 버전에서 무엇이 달랐는지 명시                |
| 사용 도구          | GA4, Amplitude, Optimizely 등 분석/실험 툴  |
| 통계 방법          | t-검정, 카이제곱, 베이지안 등 통계 분석 방식           |
| 결과 요약          | 어떤 버전이 이겼는가? 유의미했는가?                  |
| p-value / 신뢰구간 | 유의성 수치 및 효과 크기                        |
| 실행 결과          | 이 결과를 바탕으로 무엇을 실제로 적용했는가?             |
| 학습 내용          | 다음 실험에 반영할 점은 무엇인가?                   |

> 팁: 이 템플릿은 Notion/Confluence/Google Sheets로 저장하고, 실험 대시보드 및 OKR과 연결해 사용하세요.

---

## 3. 실무 운영 팁

* 실험당 하나의 **주요 지표만 설정**
* 한 번에 하나의 변경사항만 테스트 (멀티배리언트 실험 제외)
* 가설은 **실험 전** 명확히 문서화할 것
* 가드레일 지표 꼭 포함 → 사용성/성능 저하 방지
* p-value보다 효과 크기(effect size)도 함께 시각화할 것
