# Phase 3: Feature Extraction

This document describes how meaningful behavioral features were derived from the
minute-level actigraphy data after quality control.

The full executable analysis pipeline is available here:

[**actigraphy_depression_full_pipeline.ipynb**](https://github.com/hariniramalingam2320-beep/actigraphy-depression-modeling/blob/main/actigraphy_depression_full_pipeline.ipynb)

---

## Purpose of This Phase

Raw minute-by-minute activity data are high-dimensional and difficult to interpret
directly. The goal of this phase was to summarize each participant’s activity patterns
into a compact set of interpretable features that capture daily behavior and rhythm.

All features were computed at the **participant level**, resulting in one feature
vector per participant.

---

## Features Extracted

The following categories of features were derived:

### Overall Activity Level
- Mean activity
- Median activity
- Minimum and maximum activity
- Variability measures (standard deviation and variance)

### Inactivity Patterns
- Proportion of zero-activity minutes, reflecting prolonged inactivity or rest

### Day–Night Rhythm
- Day-to-night activity ratio, capturing differences between daytime and nighttime
  activity levels

### Temporal Regularity
- Intradaily variability, measuring how fragmented or irregular activity patterns are
  across the day
- Relative amplitude, reflecting the contrast between the most active and least active
  periods of the day

---

## Outcome of Phase 3

At the end of this phase, the raw actigraphy time series were transformed into a
participant-level feature dataset containing **12 behavioral features** for each of
the **55 participants**.

This feature matrix provided an interpretable representation of activity behavior and
served as the input for clinical data integration and statistical modeling in later
phases.
