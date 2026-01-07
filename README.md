# Actigraphy-Based Modeling of Depression

This repository presents a research-oriented analysis of wearable actigraphy data
to study behavioral patterns associated with depression.

The project demonstrates how minute-level activity data collected from wearable
devices can be transformed into interpretable behavioral features and linked to
clinical outcomes using simple, transparent statistical models.

---

## Project Overview

Depression is associated with changes in daily activity, rest, and circadian
rhythms. Using passively collected actigraphy data, this project examines whether
such behavioral patterns can be quantified and related to depression status and
symptom severity.

The analysis follows a clear, phase-wise workflow, from raw data organization to
statistical modeling and interpretation.

---

## Repository Structure



```text
actigraphy-depression-modeling/
├── README.md
├── actigraphy_depression_full_pipeline.ipynb
├── notebooks/
│   ├── 01_data_loading.md
│   ├── 02_quality_control.md
│   ├── 03_feature_extraction.md
│   ├── 04_clinical_data_integration.md
│   ├── 05_modeling.md
│   └── 06_results_and_interpretation.md
```



---

## Analysis Pipeline

The complete executable analysis is contained in:

- **[Actigraphy_depression_full_pipeline.ipynb](https://github.com/hariniramalingam2320-beep/actigraphy-depression-modeling/blob/main/actigraphy_depression_full_pipeline.ipynb)**

For clarity and ease of understanding, the analysis is also documented phase by
phase in the following files:

1. **[Phase 1: Data Loading](notebooks/01_data_loading.md)**  
   Organization of raw actigraphy files, participant identifiers, and group labels.

2. **[Phase 2: Quality Control](notebooks/02_quality_control.md)**  
   Validation of recording duration, sampling consistency, missing data, and
   activity value ranges.

3. **[Phase 3: Feature Extraction](notebooks/03_feature_extraction.md)**  
   Derivation of interpretable behavioral features summarizing activity level,
   inactivity, and daily rhythm regularity.

4. **[Phase 4: Clinical Data Integration](notebooks/04_clinical_data_integration.md)**  
   Merging actigraphy-derived features with clinical and demographic information.

5. **[Phase 5: Statistical Modeling](notebooks/05_modeling.md)**  
   Use of interpretable statistical models to relate behavioral features to
   depression status and severity.

6. **[Phase 6: Results and Interpretation](notebooks/06_results_and_interpretation.md)**  
   High-level interpretation of findings and discussion of implications.

---

## Data Availability

Raw actigraphy and clinical data are **not included** in this repository due to
licensing and privacy restrictions.

The dataset was obtained from publicly available research sources. Interested
users should obtain access from the original data provider through this link [Data source](https://www.kaggle.com/datasets/arashnic/the-depression-dataset?resource=download).

---

## Key Takeaways

- Wearable actigraphy data capture meaningful behavioral differences associated
  with depression
- Simple, interpretable features can summarize complex time-series data
- Activity irregularity and inactivity patterns are particularly informative
- Passive sensing offers promising tools for mental health research


