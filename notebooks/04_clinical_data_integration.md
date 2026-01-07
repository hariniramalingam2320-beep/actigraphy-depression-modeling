# Phase 4: Clinical Data Integration

This document describes how clinical and demographic information was integrated
with the actigraphy-derived features created in Phase 3.

The full executable analysis pipeline is available here:

[**actigraphy_depression_full_pipeline.ipynb**](https://github.com/hariniramalingam2320-beep/actigraphy-depression-modeling/blob/main/actigraphy_depression_full_pipeline.ipynb)

---

## Purpose of This Phase

While actigraphy features describe behavioral patterns, clinical variables provide
important context about participants’ mental health status.

The goal of this phase was to combine behavioral features with clinical data in
order to enable clinically meaningful modeling and interpretation.

---

## Clinical Data Used

Clinical and demographic information was obtained from a separate metadata file
and included variables such as:

- Participant identifier
- Age group and gender
- Diagnostic category
- Clinical severity scores (MADRS at start and end of recording)

These variables were available for participants in the condition group.

---

## What Was Done

During this phase:

- Clinical data were loaded and inspected
- Participant identifiers were used to align clinical records with actigraphy features
- Behavioral features and clinical variables were merged into a single dataset
- Changes in depression severity over the recording period were computed where applicable

Only participants with valid clinical information were included in analyses that
required clinical labels.

---

## Outcome of Phase 4

At the end of this phase, a combined dataset was created that linked each participant’s
activity-based behavioral features with relevant clinical and demographic information.

This integrated dataset enabled:
- Group-level comparisons between control and condition participants
- Modeling of depression status using actigraphy features
- Analysis of relationships between activity patterns and depression severity

The merged dataset was then used as input for statistical modeling and predictive
analysis in subsequent phases.
