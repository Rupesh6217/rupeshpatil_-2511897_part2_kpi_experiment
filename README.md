# rupeshpatil_-2511897_part2_kpi_experiment
# KPI Framework, Business Experiment Analysis & Decision Recommendation

## Student Information

**Name:** Rupesh Patil
**Student ID:** 2511897

# Business Context

A subscription-based digital product company launched a new onboarding and activation campaign to improve user conversion and early engagement.

Users were divided into two groups:

* **Control Group:** Existing onboarding experience
* **Treatment Group:** New onboarding campaign experience

The business objective is to determine whether the new onboarding campaign should be rolled out to all users based on measurable improvements in conversion and engagement metrics while ensuring no adverse impact on user experience or revenue quality.



# Business Problem Statement

The company must decide whether the new onboarding campaign should replace the existing onboarding experience.

This decision impacts:

* Product Management Team
* Marketing Team
* Revenue Operations Team
* Existing and Future Users

The primary metric expected to improve is user conversion from trial to paid subscription.

Risks that must be monitored include:

* Increased refund requests
* Higher support ticket volume
* Lower engagement quality
* Longer conversion times
* Segment-specific performance decline

Before making a recommendation, statistical evidence must demonstrate that any observed improvement is meaningful and not due to random variation.



# Dataset Description

The dataset contains user-level experiment data including:

* User ID
* Experiment Group
* Region
* Device Type
* Traffic Source
* Plan Type
* Landing Page Visit Status
* Trial Start Status
* Onboarding Completion Status
* Paid Conversion Status
* Revenue
* Refund Request Indicator
* Support Ticket Indicator
* Engagement Score
* Days to Convert

The data is used to compare performance between the Control and Treatment groups.



# North Star Metric

## Selected Metric

**Paid Conversion Rate**

### Why It Is the North Star Metric

Paid conversion directly measures the company's ability to convert users into paying customers.

It has the strongest connection to:

* Revenue growth
* Customer acquisition efficiency
* Business sustainability

### Supporting Metrics

The following metrics support the North Star Metric:

* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Average Revenue Per User
* Engagement Score
* Days to Convert

These metrics help explain why conversion changes occur but are not the primary business outcome.

### Risk of Blind Optimization

If paid conversion rate is optimized without considering other metrics:

* Refund rates may increase
* Customer satisfaction may decline
* Support workload may increase
* Low-quality users may be acquired

Therefore guardrail metrics must also be evaluated.



# KPI Tree Summary

## North Star Metric

Paid Conversion Rate

### Primary Driver 1: User Acquisition Quality

* Landing Page Visit Rate
* Traffic Source Performance

### Primary Driver 2: Activation Success

* Trial Start Rate
* Onboarding Completion Rate

### Primary Driver 3: Monetization Performance

* Revenue Per User
* Revenue Per Converted User

### Guardrail Metrics

* Refund Rate
* Support Ticket Rate
* Days to Convert
* Engagement Score

The KPI Tree is included in:

* outputs/kpi_tree.png
* screenshots/kpi_tree_preview.png



# Data Preparation and Validation

The dataset was reviewed for:

### Missing Values

Checked all columns for null or blank values.

### Duplicate User IDs

Verified user IDs for uniqueness.

### Invalid Binary Values

Validated all binary fields contain only expected values (0 or 1).

### Revenue Outliers

Reviewed unusually high revenue values.

### Group Counts

Verified sample size distribution across Control and Treatment groups.

### Segment Distribution

Compared distribution across:

* Region
* Device Type
* Traffic Source
* Plan Type

No major imbalances affecting analysis were identified.



# Experiment Analysis Approach

The following metrics were calculated and compared between Control and Treatment groups:

* User Count
* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Paid Conversion Rate
* Average Revenue Per User
* Average Revenue Per Converted User
* Refund Rate
* Support Ticket Rate
* Engagement Score
* Average Days to Convert

Additional segment-level analysis was performed using:

* Region
* Device Type
* Traffic Source

Results are included in:

outputs/experiment_summary.xlsx



# Hypothesis Test Summary

### Null Hypothesis (H₀)

There is no significant difference in paid conversion rate between the Control and Treatment groups.

### Alternative Hypothesis (H₁)

There is a significant difference in paid conversion rate between the Control and Treatment groups.

### Test Type

Two-Tailed Hypothesis Test

### Significance Level

0.05

### Decision Rule

* p-value < 0.05 → Reject H₀
* p-value ≥ 0.05 → Fail to Reject H₀

The test evaluates whether the observed improvement is statistically significant.

Detailed analysis is available in:

analysis/hypothesis_test_notes.md



# Guardrail Metrics Considered

The following guardrail metrics were evaluated:

1. Refund Rate
2. Support Ticket Rate
3. Average Days to Convert
4. Engagement Score

These metrics ensure the treatment does not improve conversion at the cost of user experience or revenue quality.



# Final Recommendation

Based on the experiment results, hypothesis testing outcomes, and guardrail metric evaluation, the treatment campaign should be implemented only if:

* Conversion rate improvement is statistically significant.
* Revenue impact is positive.
* Refund rates remain acceptable.
* Support ticket rates do not increase materially.
* No major segment-level decline is observed.

If these conditions are not met, additional testing should be conducted before full rollout.



# Assumptions

* Data accurately represents user behavior.
* Experiment groups were assigned correctly.
* Sample size is sufficient for statistical testing.
* External factors impacted both groups equally.



# Limitations

* Results are based on a single experiment period.
* User behavior may change over time.
* External market conditions may influence outcomes.
* Additional validation may be required before large-scale deployment.



# Repository Contents

## Data

* campaign_experiment_data.xlsx

## Analysis

* experiment_analysis.xlsx
* hypothesis_test_notes.md

## Outputs

* kpi_tree.png
* experiment_summary.xlsx
* recommendation_memo.md

## Screenshots

* summary_metrics.png
* hypothesis_test_output.png
* kpi_tree_preview.png



# Key Deliverables

✔ Business Problem Framing

✔ North Star Metric Definition

✔ KPI Tree

✔ Experiment Analysis

✔ Hypothesis Testing

✔ Guardrail Evaluation

✔ Decision Recommendation

✔ Documentation and Screenshots
