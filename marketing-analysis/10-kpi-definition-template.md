# KPI Definition Template

## Overview

This document provides a **comprehensive template and guidance** for defining and managing KPIs (Key Performance Indicators) in real-world marketing, growth, and product teams. Proper KPI definition is essential for cross-team alignment, clean analytics, and effective dashboard building.

---

## 1. Why KPI Definitions Matter

* Avoid misinterpretation (e.g., different meanings of "conversion" across departments)
* Align team execution with company OKRs and strategic priorities
* Enable automated dashboard integration, reduce analytics inconsistency
* Clarify communication across cross-functional teams (Product, Growth, CRM, Finance)

---

## 2. KPI Definition Table Template

| KPI Name                        | Description                                 | Formula                                    | Owner           | Source Tables                        | Update Frequency | Segmentation             | Business Context                      |
| ------------------------------- | ------------------------------------------- | ------------------------------------------ | --------------- | ------------------------------------ | ---------------- | ------------------------ | ------------------------------------- |
| CAC (Customer Acquisition Cost) | Avg cost to acquire one user                | Paid Media Spend ÷ New Users               | Growth Lead     | `ad_spend`, `signups`                | Weekly           | Channel, Campaign        | Focus on paid media only              |
| LTV (Customer Lifetime Value)   | Total revenue from a customer over lifetime | Avg monthly revenue × avg retention months | Finance         | `payments`, `users`, `subscriptions` | Monthly          | User Plan, Cohort        | Tie directly to CAC to measure ROI    |
| ARPU (Avg Revenue Per User)     | Avg revenue per active user                 | Total Revenue ÷ Active Users               | Finance Analyst | `payments`, `sessions`               | Monthly          | Geography, Segment       | Use gross revenue (not net)           |
| 7D Retention Rate               | % of users active 7 days post-signup        | D7 Active Users ÷ D0 Signups               | Product Manager | `users`, `events`                    | Weekly           | Acquisition Source       | Exclude internal/test users           |
| Conversion Rate                 | % of users completing key action            | Converters ÷ Visitors                      | CRM Lead        | `pageviews`, `events`                | Daily            | Device Type, Funnel Step | Define what qualifies as a conversion |
| NPS                             | Net Promoter Score                          | %Promoters - %Detractors                   | CX Lead         | `surveys`                            | Monthly          | Product Type             | Track changes over version releases   |

> TIP: Host this table in Notion, Confluence, or Google Sheets with version history, and assign update cycles to each KPI owner.

---

## 3. Strategic Linking with OKRs

| Objective                  | KPI            | Target | Time Frame |
| -------------------------- | -------------- | ------ | ---------- |
| Increase profitability     | CAC\:LTV Ratio | > 3.0  | Quarterly  |
| Grow active users          | DAU / MAU      | 25%+   | Monthly    |
| Improve product experience | 7D Retention   | > 40%  | Monthly    |
| Enhance user satisfaction  | NPS            | > 60   | Quarterly  |

---

## 4. Operational Best Practices

### Ownership & Version Control

* Assign a clear **owner per KPI** (not per dashboard)
* Include version dates for formula changes and logic assumptions

### Visualization Standards

* Each KPI should be **reflected in dashboards** with clear segment filters
* Use **threshold color coding** for intuitive scans (e.g., red if < goal)

### Common Mistakes

* Ambiguous definitions (e.g., unclear “active user” criteria)
* KPIs with no clear action path (e.g., tracking without purpose)
* Overloading: Tracking 20+ KPIs with no prioritization

---

# KPI 정의서 템플릿 (KPI Definition Template)

## 개요

이 문서는 마케팅, 그로스, 제품 조직에서 KPI를 **정확히 정의하고 일관되게 관리**할 수 있도록 설계된 실전 템플릿입니다. KPI 정의서는 팀 간 협업, 대시보드 연동, 분석 정확도 확보에 핵심적 역할을 합니다.

---

## 1. KPI 정의가 중요한 이유

* 팀 간 지표 해석 혼선 방지 (예: ‘전환’ 기준이 부서마다 다름)
* OKR과 실무 실행을 연계하는 도구
* 대시보드 자동화 및 분석의 기준점 제공
* 제품/그로스/CRM/재무 간 공통 언어 제공

---

## 2. KPI 정의 테이블 템플릿

| KPI명              | 설명               | 계산식                  | 담당자     | 데이터 테이블                              | 갱신 주기 | 세그먼트 기준      | 비즈니스 맥락          |
| ----------------- | ---------------- | -------------------- | ------- | ------------------------------------ | ----- | ------------ | ---------------- |
| CAC (고객 획득 비용)    | 1인당 유료 획득 비용     | 유료 광고비 ÷ 신규 가입자 수    | 그로스 리드  | `ad_spend`, `signups`                | 주간    | 채널, 캠페인      | 오가닉 제외, 유료만 포함   |
| LTV (고객 생애 가치)    | 고객 1인의 누적 매출     | 월 평균 매출 × 평균 유지 개월 수 | 재무팀     | `payments`, `users`, `subscriptions` | 월간    | 요금제, 코호트     | CAC 대비 수익성 판단 기준 |
| ARPU (사용자당 평균 매출) | 액티브 유저 1인당 평균 매출 | 총매출 ÷ 활성 사용자 수       | 재무 분석가  | `payments`, `sessions`               | 월간    | 지역, 세그먼트     | 순매출 아님, 총매출 기준   |
| 7일 리텐션            | 가입 후 7일 후 재방문율   | D7 접속 ÷ D0 가입        | PM      | `users`, `events`                    | 주간    | 유입 채널        | 내부/테스트 유저 제외     |
| 전환율               | 특정 행동 완료 비율      | 전환자 수 ÷ 방문자 수        | CRM 리드  | `pageviews`, `events`                | 일간    | 기기 유형, 퍼널 단계 | 전환 기준 명확히 기술 필요  |
| NPS               | 순추천지수            | 프로모터% - 디트랙터%        | 고객경험 담당 | `surveys`                            | 월간    | 제품 유형        | 릴리즈별 변화 추적 필요    |

> 팁: 이 테이블은 Notion/Confluence/Google Sheets에 저장하고 버전 기록 관리, 책임자별 갱신 주기 지정하는 것이 이상적입니다.

---

## 3. 전략 연계 (OKR 맵핑 예시)

| 목표 (Objective) | KPI          | 목표 수치 | 기간 |
| -------------- | ------------ | ----- | -- |
| 수익성 향상         | CAC\:LTV 비율  | > 3.0 | 분기 |
| 액티브 사용자 증가     | DAU / MAU 비율 | 25%+  | 월간 |
| 제품 경험 향상       | 7일 리텐션율      | > 40% | 월간 |
| 고객 만족 향상       | NPS 점수       | > 60  | 분기 |

---

## 4. 운영 실무 가이드

### 책임자 및 변경 이력 관리

* KPI별 **담당자 명확히 지정** (대시보드가 아닌 지표 기준)
* 공식 변경 이력 관리 및 전제 조건 명시

### 대시보드 연동 기준

* 각 KPI는 시각화 대시보드에 포함되어야 함
* 목표 대비 상태 강조 (예: 목표 미달시 빨간색 경고 등 시각적 표시)

### 자주 하는 실수

* 모호한 정의 (예: ‘활성 사용자’ 기준 불명확)
* 실행과 연결되지 않는 KPI (측정만 하고 끝나는 지표)
* 지나치게 많은 지표 → 우선순위 없는 KPI 남발
