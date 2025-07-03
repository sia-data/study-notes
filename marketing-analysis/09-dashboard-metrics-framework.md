# Dashboard Metrics Framework 

## Overview

A well-designed dashboard is not just a collection of numbers — it’s a decision-support system. It helps teams monitor product health, measure performance, and align on what matters most.

This note outlines how to design actionable marketing and product dashboards by organizing metrics into a logical framework, choosing the right visualizations, and tailoring to stakeholder needs.

---

## 1. Principles of Dashboard Design

### Goal-Driven

* Start with business questions, not tools
* Example: “How is our acquisition cost trending by channel over time?”

### Layered (3-level hierarchy)

1. **Executive KPIs** – Summary view (e.g., CAC, LTV, MRR, Retention)
2. **Operational Metrics** – Channel-level, campaign-level, funnel metrics
3. **Diagnostic Metrics** – Deep-dive (CTR, bounce rate, time on site)

### Actionable

* Highlight what requires attention (e.g., conditional formatting, alerts)
* Display trends rather than just static values

### Clean & Consistent

* Use consistent date formats, segment definitions, and units
* Avoid clutter: Limit to 5–7 charts per page

---

## 2. Metric Categories by Funnel Stage

| Funnel Stage | Key Metrics                                                             |
| ------------ | ----------------------------------------------------------------------- |
| Acquisition  | CAC, CTR, CPM, CPA, CPI, Source/Medium breakdown                        |
| Activation   | Sign-up rate, first key action (e.g., add to cart, onboarding complete) |
| Retention    | Day-1/7/30 retention, churn rate, DAU/MAU, session frequency            |
| Revenue      | ARPU, ARPPU, LTV, conversion to paying user, gross margin               |
| Referral     | Invite rate, viral coefficient (K-factor), referral conversion          |

---

## 3. Dashboard Use Cases & Tips

### Executive Dashboard

* Audience: CEO, CMO, Leadership
* Focus: High-level trends, YoY/MoM growth, revenue, CAC vs LTV
* Tool: Looker Studio, Tableau

### Performance Dashboard

* Audience: Growth, Paid Ads, CRM teams
* Focus: Campaign-level ROAS, UTM channel attribution, spend vs return
* Tool: Google Data Studio + BigQuery / GA4

### Product Dashboard

* Audience: Product managers, UX teams
* Focus: Funnel drop-off, NUX completion, feature adoption
* Tool: Amplitude, Mixpanel, GA4

---

## 4. Best Practices from Real-World Use

* **Automate data refresh** (daily or hourly if needed)
* **Annotate chart spikes/dips** with events (e.g., campaign start, bug fix)
* Use **comparison periods** (week-over-week, month-over-month)
* **Add filters** (by device, geography, user type)
* Regularly **review and prune** metrics that no longer drive decisions

---

## 5. Common Pitfalls to Avoid

* Too many vanity metrics (e.g., pageviews without context)
* Lack of ownership – nobody knows who maintains the dashboard
* Inconsistent definitions (e.g., different LTV formulas used across teams)
* One-size-fits-all dashboards for every stakeholder

---

# 대시보드 지표 설계 프레임워크 (Dashboard Metrics Framework)

## 개요

잘 설계된 대시보드는 단순히 숫자 모음이 아닌 **의사결정 지원 시스템**입니다. 팀이 제품의 상태를 모니터링하고, 마케팅 성과를 측정하며, 중요한 지표에 집중하게 해줍니다.

이 노트는 실무에서 활용 가능한 마케팅/제품 대시보드를 **논리적 구조**로 설계하고, **올바른 시각화**를 선택하며, **이해관계자 맞춤형**으로 구성하는 방법을 정리한 문서입니다.

---

## 1. 대시보드 설계의 원칙

### 목표 중심 설계

* “도구”가 아닌 “질문”에서 출발해야 함
* 예시: “채널별 CAC는 시간에 따라 어떻게 변화하고 있는가?”

### 계층적 구성 (3단계 구조)

1. **핵심 KPI** – 경영 요약 (CAC, LTV, MRR, 리텐션 등)
2. **운영 지표** – 채널별, 캠페인별, 퍼널별 지표
3. **진단 지표** – 세부 분석 (CTR, 이탈률, 체류시간 등)

### 행동 유도형 (Actionable)

* 이상 징후 강조 표시 (조건부 서식, 경고 등)
* 정적인 숫자보다 **추세** 위주 시각화

### 일관성 있는 UI

* 날짜 포맷, 지표 정의, 단위 형식 통일
* 과도한 정보 피하고, 한 페이지당 5\~7개 시각화로 제한

---

## 2. 퍼널 단계별 지표 정리

| 퍼널 단계       | 주요 지표                              |
| ----------- | ---------------------------------- |
| Acquisition | CAC, CTR, CPM, CPA, CPI, 유입 채널 비율  |
| Activation  | 가입율, 첫 행동 수행율 (장바구니 담기, 온보딩 완료 등)  |
| Retention   | 1일/7일/30일 리텐션, 이탈률, DAU/MAU, 세션 빈도 |
| Revenue     | ARPU, ARPPU, LTV, 유료전환율, 매출 총이익률   |
| Referral    | 초대율, 바이럴 계수(K-factor), 추천 가입 전환율   |

---

## 3. 대시보드 유형별 구성 예시

### 경영용 대시보드

* 대상: CEO, CMO, 임원
* 목적: 전체 성과, 월별/연도별 성장률, CAC 대비 LTV
* 도구 예: Looker Studio, Tableau

### 마케팅 성과 대시보드

* 대상: Growth 팀, 퍼포먼스 마케터, CRM 담당자
* 목적: ROAS, UTM별 채널 분석, 캠페인 성과 측정
* 도구 예: Google Data Studio + BigQuery, GA4

### 제품팀 대시보드

* 대상: PO, UX 팀
* 목적: 퍼널 이탈 분석, 온보딩 완료율, 기능 도입률 추적
* 도구 예: Amplitude, Mixpanel, GA4

---

## 4. 실무에서의 베스트 프랙티스

* **자동 데이터 업데이트** 설정 (일간, 필요시 시간 단위)
* 지표 변화에 대해 **주석 처리** (캠페인 시작, 버그 수정 등)
* **비교 시계열** 제공 (주간/월간 전환율 추이 등)
* **필터 기능** 추가 (기기, 지역, 사용자 유형)
* **의사결정에 기여하지 않는 지표는 정기적으로 정리/삭제**

---

## 5. 자주 발생하는 실수

* 허영 지표 위주 구성 (예: 문맥 없는 페이지뷰)
* 책임자 부재 (누가 관리하는지 모름)
* 지표 정의 불일치 (LTV 공식을 팀별로 다르게 사용)
* 모든 사람에게 동일한 대시보드 제공 (사용자 맞춤 부재)
