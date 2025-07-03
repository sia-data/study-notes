# Acquisition Metrics

## What is Acquisition?

**Acquisition** refers to the process of attracting new users to your product or service. This stage is focused on how potential users discover and enter your funnel.

Understanding acquisition is critical because it:

* Helps determine which channels are effective.
* Informs budget allocation decisions.
* Enables long-term growth planning based on user quality.

## Key Metric: CAC (Customer Acquisition Cost)

**CAC** is the average cost to acquire one paying customer. It’s essential for evaluating marketing efficiency.

### CAC Formula:

CAC = Total Marketing Spend / Number of Customers Acquired

To properly calculate CAC:

* Track spending per channel/campaign.
* Attribute conversions accurately to acquisition sources.

**Important:** CAC must be lower than **LTV** (Lifetime Value) to ensure sustainable growth.

> "If CAC = LTV, it's break-even. If CAC > LTV, it's unprofitable."

Often, **increasing LTV** is more effective than reducing CAC.

## Acquisition Tracking Methods

### 1. Web – UTM Parameters

UTM (Urchin Tracking Module) parameters are tags added to URLs to identify traffic sources.

Example:

```
https://yourdomain.com?utm_source=facebook&utm_medium=blog_article&utm_campaign=launch&utm_term=quarter_two&utm_content=header_link
```

| Parameter     | Description                 | Example       |
| ------------- | --------------------------- | ------------- |
| utm\_source   | Where the traffic came from | facebook      |
| utm\_medium   | The type of channel         | blog\_article |
| utm\_campaign | Name of the campaign        | launch        |
| utm\_term     | Search keyword (if any)     | quarter\_two  |
| utm\_content  | Specific content variation  | header\_link  |

Tools: [Google Campaign URL Builder](https://ga-dev-tools.web.app/campaign-url-builder/)

### 2. Mobile App – Attribution Tools

Unlike the web, UTM parameters are lost when traffic goes through the App Store.
Use mobile attribution tools to track installs and link them to original marketing channels.

Examples: AppsFlyer, Adjust, Branch, Singular

These tools help identify:

* Which campaigns led to installs
* LTV and retention per channel

## Paid Acquisition Metrics

| Metric                    | Description                                 |
| ------------------------- | ------------------------------------------- |
| CPC (Cost Per Click)      | Cost per ad click                           |
| CPI (Cost Per Install)    | Cost per app install                        |
| CPA (Cost Per Action)     | Cost per desired user action (e.g., signup) |
| CPM (Cost Per Mille)      | Cost per 1,000 impressions                  |
| CPP (Cost Per Period)     | Fixed cost for time-based ads               |
| ROAS (Return on Ad Spend) | Revenue generated per dollar spent          |

## Success Benchmark

For acquisition to be efficient:

```
CAC < LTV (Customer Lifetime Value)
```

Segment CAC by:

* Channel
* Campaign
* Time period

This enables smarter budget decisions:
"Which campaign on which channel performed best in Q1?"

## Attribution Caveats

* **Last-click attribution** can be misleading. Use multi-touch models if possible.
* Cross-device and offline conversions require advanced tracking or manual calibration.

## Acquisition → Activation Funnel Example

```
Ad Impressions: 1,000,000
Ad Clicks: 10,000 → CTR = 1%
App Installs: 5,000 → Install Rate = 50%
Game Starts: 4,000 → Activation Rate = 80%
```

> Improve where drop-off is highest or where cost per conversion is too high.

---

# 획득 지표 (Acquisition Metrics)

## Acquisition이란?

**획득**은 신규 사용자가 우리 서비스를 발견하고 유입되는 과정이다. 퍼널의 가장 첫 단계로, **사용자가 어떻게 우리를 알게 되었는지**가 핵심.

획득 분석이 중요한 이유:

* 어떤 채널이 효과적인지 파악 가능
* 마케팅 예산 분배 전략 수립
* 장기적 성장 기반 마련 (유저 질 판단 가능)

## 핵심 지표: CAC (Customer Acquisition Cost)

**CAC**는 1명의 유료 고객을 획득하기 위해 소요되는 평균 비용. 마케팅 효율성을 판단하는 주요 지표이다.

### CAC 공식:

CAC = 총 마케팅 비용 / 획득한 고객 수

정확한 CAC 측정을 위해:

* 채널, 캠페인 단위로 예산 집행 내역 추적
* 유입 및 전환 경로를 정확히 추적

> CAC는 \*\*LTV (고객 생애 가치)\*\*보다 작아야 비즈니스가 지속 가능함

대개 CAC를 낮추는 것보다 **LTV를 높이는 전략**이 더 효과적임

## 획득 추적 방법

### 1. 웹 – UTM 파라미터

UTM은 URL 뒤에 붙는 태그로, 유입 트래픽의 출처를 파악할 수 있게 해준다다.

예시:

```
https://yourdomain.com?utm_source=facebook&utm_medium=blog_article&utm_campaign=launch&utm_term=quarter_two&utm_content=header_link
```

| 파라미터          | 의미        | 예시            |
| ------------- | --------- | ------------- |
| utm\_source   | 유입 출처     | facebook      |
| utm\_medium   | 유입 매체 유형  | blog\_article |
| utm\_campaign | 캠페인 이름    | launch        |
| utm\_term     | 검색 키워드    | quarter\_two  |
| utm\_content  | 콘텐츠 세부 구분 | header\_link  |

도구: [Google Campaign URL Builder](https://ga-dev-tools.web.app/campaign-url-builder/)

### 2. 앱 – 어트리뷰션 도구

앱스토어 경로를 거치며 UTM이 유실되므로, 앱 설치와 전환 추적에는 별도의 어트리뷰션 툴이 필요함.

예: AppsFlyer, Adjust, Branch, Singular

이 도구들을 통해:

* 어떤 캠페인이 설치를 유도했는지 분석
* 채널별 LTV, 리텐션 등 성과 측정

## 유료 광고 지표

| 지표                         | 의미               |
| -------------------------- | ---------------- |
| CPC (Cost Per Click)       | 클릭당 광고비          |
| CPI (Cost Per Install)     | 설치당 광고비          |
| CPA (Cost Per Action)      | 특정 액션(가입 등)당 광고비 |
| CPM (Cost Per Mille)       | 1,000회 노출당 광고비   |
| CPP (Cost Per Period)      | 기간형 광고 단가        |
| ROAS (Return On Ads Spend) | 광고비 대비 수익        |

## 성공 기준

```
CAC < LTV (고객 생애 가치)
```

세분화된 CAC 분석은 다음 기준으로:

* 채널 별
* 캠페인 별
* 기간 별

이렇게 나누면:
“1분기 동안 가장 효율적인 캠페인은 무엇이었는가?”와 같은 질문에 답할 수 있음

## 어트리뷰션 주의점

* **라스트 클릭(Last-click)** 모델은 편향적일 수 있음
* 가능하다면 멀티 터치 어트리뷰션 모델 활용
* 크로스디바이스, 오프라인 전환은 별도 추적 방식 필요

## 퍼널 예시: 획득 → 실행

```
광고 노출: 1,000,000
광고 클릭: 10,000 → 클릭율: 1%
앱 설치: 5,000 → 설치율: 50%
게임 실행: 4,000 → 실행율: 80%
```

> 전환율이 낮거나 전환 비용이 높은 구간부터 개선할 것

