# A/B Testing Framework

## What is A/B Testing?

**A/B testing** is a method of comparing two versions of a variable (e.g., UI layout, copy, feature) to determine which performs better. It’s a controlled experiment where users are randomly split into two (or more) groups.

A/B testing helps:

* Validate design or feature hypotheses
* Optimize conversion rates
* Minimize risk before full rollout

## Step-by-Step A/B Testing Framework

### 1. Define the Problem

Understand the **goal** and the **metric** to measure.

Example:

* Observation: Users who click recommended products tend to spend more, but click-through rate is low.
* Goal: Increase engagement with recommended products.

### 2. Set Success, Supporting, and Guardrail Metrics

| Metric Type            | Definition                     | Example                              |
| ---------------------- | ------------------------------ | ------------------------------------ |
| Primary (Success)      | Core business outcome          | ARPU, conversion rate                |
| Secondary (Supporting) | Related behavioral metric      | Clicks on recommended products       |
| Guardrail              | Prevents negative side-effects | Bounce rate, load time, revenue drop |

Also check for **sample ratio mismatch** to ensure groups are evenly split.

### 3. Formulate a Hypothesis

Example Hypothesis:

> Showing recommended products on product detail pages will increase ave다.
