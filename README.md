
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Psychometric Validation of the Perceived Stress Scale

## Overview

This project validates the Perceived Stress Scale (PSS) among Black
adolescents in the U.S., using data from the National Survey of American
Life – Adolescent Supplement (NSAL-A). This analysis evaluates the
factor structure, measurement invariance, and predictive validity of the
PSS-14, PSS-13, and PSS-10 to improve stress measurement and inform
youth mental health interventions.

## Objectives

Validate the CFA structure of the PSS-14, PSS-13, and PSS-10 Examine
measurement invariance across gender (Configural, Metric, Scalar) Assess
predictive validity for Major Depressive Disorder (MDD) using ROC
analysis

\#️# Methods & Tools

- Libraries: RMarkdown, tidyverse, lavaan, semTools, psych, pROC, DT,
  lavaanPlot, naniar, reshape2, plotly
- Statistical Analyses:
  - Confirmatory Factor Analysis (CFA)
  - Model Comparison: 1-Factor vs. 2-Factor
  - Measurement Invariance by Gender
  - Predictive Validity (ROC curve and AUC)

## Data:

-National Survey of American Life – Adolescent Supplement (N = 1,170
Black adolescents aged 13–17) Source: [ICPSR
\#20240](https://www.icpsr.umich.edu/web/RCMD/studies/36380)

## Key Findings

- The 2-factor model (coping + distress) outperformed the unidimensional
  model for all PSS versions. Item 12 (PC4L) showed weak loadings and
  was removed in the PSS-13 version.
- Measurement invariance across gender was supported, confirming scale
  fairness.
- Perceived Distress subscale achieved the highest predictive accuracy
  for MDD (AUC ≈ 0.78).

## Recommendations

- Use PSS-13 (without item 12) for better model fit in Black adolescent
  populations.
- Prioritize Perceived Distress subscale in clinical risk screening for
  depression.
- Avoid reliance on total scores alone; subscales provide better
  construct representation.
- Maintain gender equity in interpretation.

## How to Run the Analysis

- Open the RMarkdown file: pss_validation.Rmd
- Run in RStudio or RMarkdown environment
- Install required packages: if (!require("pacman"))
  install.packages("pacman") pacman::p_load(tidyverse, lavaan, semTools,
  semPlot, psych, pROC, naniar, haven, apaTables, reshape2, lavaanPlot,
  scales, flextable, DT)
- Knit the .Rmd file to generate the HTML report with interactive tables
  and graphs. Note: You need to download the data from the
  [source](https://www.icpsr.umich.edu/web/RCMD/studies/36380)

## Outputs

- Heatmaps of item correlations
- CFA model diagrams with standardized loadings
- Measurement invariance fit summaries
- ROC curves (PSS-13 and PSS-10) with AUC stats
