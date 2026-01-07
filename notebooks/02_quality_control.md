# Phase 2: Data Quality Control

This document summarizes the quality control checks performed on the structured
actigraphy dataset created in Phase 1.

The full executable analysis pipeline is available here:

[**actigraphy_depression_full_pipeline.ipynb**](https://github.com/hariniramalingam2320-beep/actigraphy-depression-modeling/blob/main/actigraphy_depression_full_pipeline.ipynb)

---

## What Was Checked

After loading and structuring the data, several quality checks were performed to
ensure the dataset was suitable for downstream analysis.

The following aspects were examined:

- Number of participants in each group (control vs condition)
- Total recording duration for each participant
- Consistency of the one-minute sampling interval
- Presence of missing time points
- Distribution and range of activity values
- Proportion of zero-activity (inactive) minutes

---

## Key Observations

- The dataset included **55 participants** (32 controls and 23 condition participants)
- All participants had multiple days of continuous recordings
- The expected **one-minute time resolution** was preserved across participants
- Missing time points were minimal and rare
- Activity values were within plausible ranges, with no invalid or negative values
- A substantial proportion of zero-activity minutes was observed, which is expected
  and meaningful in actigraphy data (e.g., rest or sleep periods)

---

## Outcome of Phase 2

The quality control analysis indicated that the dataset was **internally consistent**
and **sufficiently complete** for further analysis.

No aggressive data cleaning, filtering, or imputation was required. The dataset was
therefore carried forward as-is into feature extraction and modeling phases.
