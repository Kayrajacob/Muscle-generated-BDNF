# Muscle-generated-BDNF
## 1. Project Overview
This repository contains a Google Colab notebook reproducing the muscle-specific *Bdnf* knockout (MBKO) phenotype and *Pink1* expression trends from Ahuja et al. (2021) using simulated data modeled after the authors' public findings.
## 2. Main Result
Comparison of muscle *Pink1* mRNA relative expression levels between Control and MBKO female mice under High-Fat Diet (HFD) conditions:
| Metric / Group | Paper Reported Value (Approx.) | Reproduction Output | Match Direction? |
| --- | --- | --- | --- |
| **Control Expression** | ~1.00 | **1.00** | — |
| **MBKO Expression** | ~0.45–0.50 | **0.48** | Yes ($\downarrow$) |
| **Statistical Test** | $p < 0.05$ | **$p = 0.0048$** | Yes |
## 3. Exploratory Analysis & Findings
* **Findings:** A strong negative correlation ($r = -0.936, p < 0.0001$) was found between body weight gain and relative *Pink1* expression. Higher weight gain strongly associated with lower mitophagy gene expression.
## 4. Differences from Original Method & Limitations
* **Simulated vs. Raw Data:** The authors did not release a raw individual replicate CSV matrix; dataset values were simulated to match reported summary statistics and sample sizes.
* **Correlation vs. Causation:** The correlation analysis treats weight gain and *Pink1* repression as co-occurring variables, which shows an association but does not prove direct biological causality.
* **Statistical Sensitivity:** Non-parametric testing (Mann-Whitney U) on small subsets showed reduced power ($p = 0.3333$) compared to standard parametric $t$-tests ($p = 0.0048$), highlighting sensitivity to sample size assumptions.
## 6. Citation & Data Source
Ahuja, P., Ng, C. F., Pang, B. P. S., Chan, W. S., Tse, M. C. L., Bi, X., ... & Chan, C. B. (2021). *Muscle-generated BDNF (brain derived neurotrophic factor) maintains mitochondrial quality control in female mice*. Autophagy, 18(6), 1367-1384. DOI: [10.1080/15548627.2021.1985257](https://doi.org/10.1080/15548627.2021.1985257)
