# PhenoCrit: Clinical Aging and Biological Artifacts Framework <img src="man/figures/logo.png" align="right" height="139" />

[![R-CMD-check](https://github.com/andrelau0622/PhenoCrit/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/andrelau0622/PhenoCrit/actions/workflows/R-CMD-check.yaml)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
**PhenoCrit** is an open-source R toolkit designed to quantify biological aging and physiological stress trajectories in critically ill cohorts. 

Unlike conventional biological clocks (e.g., BioAge) that rely on population-based baselines, **PhenoCrit** is specifically engineered for the Intensive Care Unit (ICU). It utilizes **Functional Principal Component Analysis (FPCA)** and **Generalized Additive Models (GAM)** to dynamically decouple underlying biological deterioration from clinical intervention artifacts (e.g., fluid resuscitation, mechanical ventilation, vasoactive drugs).

##  Key Features

* **Multidimensional Profiling:** Computes biological age scores across **9 physiological dimensions** (1 Overall, 3 Systemic, 5 Organ-specific).
* **Treatment Debiasing:** Employs the **CABA (Clinical Aging and Biological Artifacts)** algorithm to strip away treatment-induced phenotypic noise.
* **Dynamic Trajectories:** Incorporates longitudinal monitoring of organ failure sequences via FPCA.
* **Prognostic Precision:** Provides superior mortality risk stratification compared to raw uncalibrated phenotypes.

---

##  Installation

You can install the development version of PhenoCrit from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("andrelau0622/PhenoCrit")
