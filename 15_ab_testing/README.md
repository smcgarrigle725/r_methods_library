# 15 · A/B Testing and Experimental Design

The final folder closes the loop between study design and analysis. The central message: decisions made before data collection — what effect size matters, how many observations are needed, how interim analyses will be handled — determine the validity of everything that follows.

| Notebook | Description |
|---|---|
| `power_analysis_R.ipynb` | Sample size calculation for t-tests, proportions, ANOVA, correlations; power curves; sensitivity analysis |
| `ab_testing_fundamentals_R.ipynb` | Two-sample tests for continuous and binary outcomes; effect sizes; permutation testing with `infer` |
| `multiple_testing_correction_R.ipynb` | Bonferroni, Holm, Benjamini-Hochberg FDR; when each is appropriate; p-value histogram diagnostics |
| `experiment_design_principles_R.ipynb` | CRD vs. RCBD; stratified randomisation; balance checks with SMD; pseudoreplication |
| `sequential_testing_R.ipynb` | α-spending functions; O'Brien-Fleming and Pocock boundaries; the true cost of peeking; `gsDesign` |
| `minimum_detectable_effect_R.ipynb` | Defining MDEs from domain knowledge; MDE vs. n curves; sensitivity to σ misspecification |
| `bayesian_ab_testing_R.ipynb` | Beta-binomial and normal-normal models; P(B > A); expected loss; prior sensitivity analysis |
| `factorial_designs_R.ipynb` | 2×2 and 3-factor factorial designs; interaction detection; Type III ANOVA; `emmeans` simple effects |

**Key packages:** `pwr`, `infer`, `gsDesign`, `bayesAB`, `emmeans`, `agricolae`, `effectsize`

---

## Applications by Sector

| Sector | Example |
|---|---|
| **Ecology** | Field experiment design for habitat manipulation; treatment/control plot randomization; testing restoration intervention effects |
| **Healthcare** | Clinical trial design; comparing treatment arms; evaluating screening protocol efficacy |
| **Finance** | Testing impact of a product change on transaction volume; evaluating a new pricing model |
| **Insurance** | Testing a new underwriting rule on claim rates; evaluating a customer communication intervention |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "pwr", "statsmodels"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
