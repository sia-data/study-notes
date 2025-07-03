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
3. **Diagnostic Metrics** – Deep-dive (CTR, bounce rate, time on site, step-by-step funnel drop-off)

### Actionable

* Highlight what requires attention (e.g., conditional formatting, alerts)
* Display trends, not just static values

### Clean & Consistent

* Use consistent date formats, segment definitions, and units
* Avoid clutter: Limit to 5–7 charts per page
* Use color coding and layout grouping

---

## 2. Metric Categories by Funnel Stage

| Funnel Stage | Key Metrics                                                                            |
| ------------ | -------------------------------------------------------------------------------------- |
| Acquisition  | CAC, CTR, CPM, CPA, CPI, Source/Medium breakdown                                       |
| Activation   | Sign-up rate, NUX completion, first action time, onboarding drop-off                   |
| Retention    | Day-1/7/30 retention, churn rate, DAU/MAU, cohort-based retention, sticky factor       |
| Revenue      | ARPU, ARPPU, LTV, conversion to paying user, gross margin, MRR (for SaaS)              |
| Referral     | Invite rate, viral coefficient (K-factor), referral conversion, invite acceptance rate |

---

## 3. Visualizing Key Metrics

### Suggested Structures

| Metric            | Chart Type                  | Reason                                      |
| ----------------- | --------------------------- | ------------------------------------------- |
| Retention (Day-N) | Cohort heatmap / line chart | Show retention decay and cohort differences |
| Funnel conversion | Step funnel chart           | Visualize where users drop off              |
| LTV vs CAC        | Line + bar combo            | Compare value vs cost across cohorts        |
| DAU / MAU         | Trend line                  | Engagement stickiness over time             |
| Campaign ROAS     | Bar chart (by channel)      | Compare performance across paid sources     |

### Dashboard Filters to Include

* Time (daily/weekly/monthly)
* Platform (web/app)
* User type (new/returning)
* Geography / device

---

## 4. Context-Specific KPI Recommendations

### SaaS (Subscription Business)

* Core: MRR, Churn Rate, LTV, CAC, ARPU
* UX: Onboarding completion, feature adoption, time-to-value
* Retention: Rolling retention, support ticket volume

### E-commerce

* Core: AOV, Conversion Rate, Cart Abandonment Rate, ARPPU, CAC
* UX: Product page views/session, time on site, bounce rate
* Retention: Repeat purchase rate, reorder interval, loyalty tier engagement

### Mobile App (Freemium or Paid)

* Core: DAU/MAU, Retention (Day 1, 7, 30), In-app purchase conversion
* UX: Onboarding drop-off, session length, screen flows
* Revenue: Subscription conversion, average revenue per install (ARPI)

---

## 5. Dashboard Use Cases & Tools

### Executive Dashboard

* Audience: CEO, CMO, Leadership
* Focus: High-level trends, YoY/MoM growth, revenue, CAC vs LTV
* Tool: Looker, Tableau, Power BI

### Performance Dashboard

* Audience: Growth, Paid Ads, CRM teams
* Focus: Campaign ROAS, UTM attribution, cost vs return
* Tool: GA4 + BigQuery, Google Data Studio, Metabase

### Product Dashboard

* Audience: PMs, Designers, UX Researchers
* Focus: Funnel drop-off, NUX flow, feature usage
* Tool: Amplitude, Mixpanel, Heap, GA4

---

## 6. Best Practices from Real-World Use

* **Automate data refresh** (daily or hourly)
* **Annotate chart spikes/dips** with contextual events
* Add **period comparisons** (WoW, MoM, vs baseline)
* Enable **interactive filters** (device, country, user cohort)
* **Review dashboards quarterly** – clean out unused metrics

---

## 7. Common Pitfalls to Avoid

* Vanity metrics without impact (e.g., pageviews alone)
* Lack of ownership or updates
* Inconsistent definitions (e.g., different LTV logic)
* Too generic – not tailored to use case or user

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
3. **진단 지표** – 세부 분석 (CTR, 이탈률, 체류시간, 퍼널 이탈 단계 등)

### 행동 유도형 (Actionable)

* 이상 징후 강조 표시 (조건부 서식, 경고 등)
* 정적인 숫자보다 **추세 위주** 시각화 필요

### 일관성 있는 UI

* 날짜 포맷, 지표 정의, 단위 형식 통일
* 과도한 정보 피하고, 한 페이지당 5\~7개 시각화로 제한
* 색상 통일 및 구간별 시각화 정렬

---

## 2. 퍼널 단계별 지표 정리

| 퍼널 단계       | 주요 지표                                                  |
| ----------- | ------------------------------------------------------ |
| Acquisition | CAC, CTR, CPM, CPA, CPI, 유입 채널 비율                      |
| Activation  | 가입율, 온보딩 완료율, 첫 행동 소요 시간, 이탈 위치                        |
| Retention   | 1일/7일/30일 리텐션, 이탈률, DAU/MAU, 코호트 기반 리텐션, sticky factor |
| Revenue     | ARPU, ARPPU, LTV, 유료전환율, 총이익률, MRR(SaaS 기준)            |
| Referral    | 초대율, 바이럴 계수(K-factor), 추천 가입 전환율, 초대 수락율               |

---

## 3. 시각화 방식 추천

| 지표          | 차트 유형            | 이유                   |
| ----------- | ---------------- | -------------------- |
| 리텐션 (Day-N) | 코호트 히트맵 / 선형 그래프 | 시계열 감쇠 및 그룹 간 차이 시각화 |
| 퍼널 전환       | 퍼널 스텝 차트         | 단계별 이탈 구조 직관적으로 표현   |
| LTV vs CAC  | 혼합형(선+막대)        | 가치와 비용의 균형 비교        |
| DAU/MAU     | 추세선              | 사용자 활동성 변동 추이 파악     |
| 캠페인 ROAS    | 막대그래프            | 채널별 수익성과 효율 비교       |

### 필터 구성 예시

* 시간 범위 (일/주/월)
* 플랫폼 (웹/앱)
* 유저 유형 (신규/기존)
* 지역/기기 종류 등

---

## 4. 상황별 KPI 추천

### SaaS (구독 기반)

* 핵심: MRR, 이탈률(Churn Rate), LTV, CAC, ARPU
* UX: 온보딩 완료율, 기능 사용률, TTV (Time To Value)
* 리텐션: Rolling retention, CS 문의량 등

### 이커머스

* 핵심: AOV(객단가), 전환율, 장바구니 이탈률, ARPPU, CAC
* UX: 제품 상세페이지 조회수/세션, 체류시간, 이탈률
* 리텐션: 재구매율, 재구매 주기, 로열티 프로그램 참여율

### 모바일 앱

* 핵심: DAU/MAU, 리텐션 (1일/7일/30일), 인앱 결제 전환율
* UX: 온보딩 이탈률, 세션 길이, 화면 이동 흐름
* 수익: 구독 전환율, 설치당 평균 수익 (ARPI)

---

## 5. 대시보드 유형 및 툴 예시

### 경영용 대시보드

* 대상: CEO, CMO, 경영진
* 핵심: 전체 성과, 전년/전월 대비 성장률, CAC-LTV
* 도구: Looker, Tableau, Power BI

### 마케팅 성과 대시보드

* 대상: Growth/광고/CRM 실무자
* 핵심: 캠페인별 ROAS, UTM 채널 분석, 비용 대비 수익
* 도구: GA4 + BigQuery, Data Studio, Metabase

### 제품 대시보드

* 대상: PM, 디자이너, UX팀
* 핵심: 퍼널 이탈 분석, 온보딩 흐름, 기능 사용률
* 도구: Amplitude, Mixpanel, Heap, GA4

---

## 6. 실무 베스트 프랙티스

* **데이터 자동화** (일간/시간 단위)
* **이벤트 기반 주석 처리** (버그 수정, 캠페인 등)
* **기간별 비교** 제공 (전주, 전월 등 기준선 설정)
* **인터랙티브 필터 제공** (기기, 지역, 유저 그룹 등)
* **정기적 대시보드 정리** (불필요 지표 제거)

---

## 7. 자주 하는 실수

* 허영 지표 중심 (예: 문맥 없는 페이지뷰)
* 지표 책임자 없음 → 업데이트 누락
* 지표 정의 불일치 (LTV 공식을 팀마다 다르게 해석)
* 타깃 없이 만든 범용 대시보드 → 실효성 낮음
