# Phase 5: Statistical Modeling

This document summarizes the statistical modeling performed using the integrated
behavioral and clinical dataset.

The full executable analysis pipeline is available here:

[**actigraphy_depression_full_pipeline.ipynb**](https://github.com/hariniramalingam2320-beep/actigraphy-depression-modeling/blob/main/actigraphy_depression_full_pipeline.ipynb)

---

## Purpose of This Phase

The goal of this phase was to examine whether activity-based behavioral features
derived from actigraphy data could:

- Distinguish between control and condition participants
- Relate to the severity of depressive symptoms

Simple and interpretable models were chosen to emphasize understanding over
prediction performance.

---

## Modeling Approach

Two main modeling strategies were used:

- **Logistic regression** to model group membership (control vs condition)
- **Linear regression (with regularization)** to examine relationships between
  behavioral features and depression severity scores

All models were trained using participant-level feature data.

---

## What Was Done

During this phase:

- Behavioral features were standardized where appropriate
- Models were fit using actigraphy-derived features as predictors
- Model coefficients were examined to understand feature contributions
- Cross-validation was used to ensure robustness of results

No complex black-box models were used, in order to retain interpretability.

---

## Outcome of Phase 5

The modeling results indicated that certain actigraphy-derived features,
particularly those related to inactivity and daily rhythm regularity,
contributed meaningfully to distinguishing between groups.

These results suggest that wearable activity patterns contain clinically
relevant signals associated with depression and motivated further interpretation
and visualization in the final phase.
