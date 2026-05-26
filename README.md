# EEG dDTF Analysis Pipeline

An end-to-end Python processing pipeline designed to handle EEG data from the open-source LEMON dataset. This workflow aims to assess cognitive reserve by computing dynamic Directed Transfer Function (dDTF) brain networks and evaluating group-level differences using Network-Based Statistics (NBS) and analysis of variance (ANOVA).

## 👤 Author
* **Author:** Einez Wu
* **Pipeline Release/Snapshot Date:** May 22nd, 2026

## 🎯 Project Goal
To design and evaluate a reproducible pipeline for analyzing raw and preprocessed EEG data. By leveraging directed functional connectivity networks across different subject demographics, this toolkit extracts network topologies to model cognitive dynamics.

## 🚀 Key Features
1. **Data Preprocessing & Structuring:** Automated cohort grouping, path management, and spatial interpolation of missing EEG channels using MNE-Python.
2. **dDTF Network Connectivity Construction:** Computes time-varying directed connectivity matrices utilizing adaptations of the algorithms formulated by [ChiShengChen](https://github.com/ChiShengChen/dDTF).
3. **Statistical Evaluation & Graph Analysis:** Employs Network-Based Statistics (NBS) alongside parametric tests like ANOVA to compare structural brain network fluctuations across subject cohorts.
4. **Data Visualization:** Built-in exploratory statistics, frequency-distribution histograms, and topographical artifact analysis plots.

## 🛠️ Requirements & Installation

The project runs on Python 3.12+ and relies heavily on the **MNE** library for neural signal engineering alongside standard data analysis packages.

Install the necessary dependencies directly via pip:

```bash
pip install mne numpy scipy matplotlib tqdm pooch requests
