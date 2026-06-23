# Hypothesis Test Notes

## Objective

The purpose of this experiment is to determine whether the new onboarding and activation campaign (Treatment Group) improves the Paid Conversion Rate compared to the existing onboarding experience (Control Group).

## Metric Being Tested

**Paid Conversion Rate**

Formula:

Paid Conversion Rate = (Number of Paid Conversions / Total Users) × 100

This metric was selected because it directly measures the success of the onboarding campaign in converting users into paying customers and has a direct impact on business revenue.


## Hypotheses

### Null Hypothesis (H₀)

There is no significant difference in Paid Conversion Rate between the Control Group and the Treatment Group.

H₀: p₁ = p₂

### Alternative Hypothesis (H₁)

The Treatment Group has a higher Paid Conversion Rate than the Control Group.

H₁: p₂ > p₁

where:

* p₁ = Paid Conversion Rate of Control Group
* p₂ = Paid Conversion Rate of Treatment Group


## Test Type

One-Tailed A/B Test

A one-tailed test is used because the business objective is specifically to determine whether the new campaign performs better than the existing experience.


## Significance Level

α = 0.05 (5%)

This means there is a 5% risk of incorrectly concluding that the Treatment Group is better when it is not.


## Test Inputs

| Metric           | Control        | Treatment      |
| ---------------- | -------------- | -------------- |
| Total Users      | [Insert Value] | [Insert Value] |
| Paid Conversions | [Insert Value] | [Insert Value] |
| Conversion Rate  | [Insert Value] | [Insert Value] |


## Decision Rule

* If p-value < 0.05 → Reject H₀
* If p-value ≥ 0.05 → Fail to Reject H₀


## Test Result

P-value: [Insert Calculated Value]

Decision:
[Reject H₀ / Fail to Reject H₀]


## Business Interpretation

If the p-value is below 0.05, the Treatment Group demonstrates a statistically significant improvement in Paid Conversion Rate. This provides evidence that the new onboarding campaign performs better than the existing experience and may be considered for rollout.

If the p-value is greater than or equal to 0.05, there is insufficient evidence to conclude that the Treatment Group performs better, and further testing may be required.

## Guardrail Considerations

The final recommendation should not be based solely on conversion improvement. The following guardrail metrics must also be reviewed:

* Refund Rate
* Support Ticket Rate
* Average Engagement Score
* Average Days to Convert

A rollout recommendation should only be made if the Treatment Group improves conversion without creating unacceptable business risks.
