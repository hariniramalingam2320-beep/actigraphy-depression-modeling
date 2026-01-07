# Phase 1: Data Loading

This document describes how raw actigraphy data were loaded and structured for analysis.  
The full executable analysis pipeline is available here:

[**actigraphy_depression_full_pipeline.ipynb**](https://github.com/hariniramalingam2320-beep/actigraphy-depression-modeling/blob/main/actigraphy_depression_full_pipeline.ipynb)

---

## Dataset Description

The dataset consists of minute-level activity recordings collected using wearable
actigraphy devices. Each participant has an individual CSV file containing:

- timestamp (one-minute intervals)
- date of measurement
- activity value recorded by the device

Participants are divided into two groups:
- **Control group**: healthy individuals
- **Condition group**: individuals diagnosed with depression

In total, the dataset includes recordings from **55 participants**, collected over
multiple days, capturing daily activity and rest patterns.

---

## What Was Done

During this phase, the raw actigraphy files were prepared for analysis:

- All participant CSV files were loaded
- Participant identifiers were extracted from file names
- Group labels (control / condition) were assigned
- Timestamps were parsed into a standard datetime format
- All participant data were combined into a single unified dataset

No data cleaning or filtering was performed at this stage.

---
## Outcome of Phase 1

At the end of this phase, all participant files were successfully loaded and
combined into a single structured dataset with consistent timestamp formatting,
participant identifiers, and group labels.

This unified dataset served as the input for quality control, feature extraction,
and modeling in later phases.

