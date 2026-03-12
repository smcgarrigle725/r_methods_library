# 03 · Mixed Effects Models

Models for clustered, nested, and longitudinal data where observations are not independent. Random effects account for grouping structure; fixed effects estimate population-level parameters.

| Notebook | Description |
|---|---|
| `random_intercept_R.ipynb` | Random intercepts for grouped data; ICC; `lme4::lmer` |
| `random_slope_R.ipynb` | Random slopes; when and why group-level effects vary; correlation of random effects |
| `crossed_random_effects_R.ipynb` | Crossed vs. nested random effects; multiple grouping factors |
| `glmm_R.ipynb` | Generalised LMMs for binary and count outcomes; `glmer` |
| `lmm_model_selection_R.ipynb` | REML vs. ML; LRT for random and fixed effects; AIC comparison |
| `rcb_designs.ipynb` | Randomised complete block designs; blocking rationale; Latin squares; Tukey's test for non-additivity |
| `repeated_measures_anova.ipynb` | Classical repeated measures ANOVA; Mauchly's sphericity test; Greenhouse-Geisser and Huynh-Feldt corrections; contrast with LMM approach |
| `split_plot_designs.ipynb` | Split-plot (partly nested) designs; between- and within-subjects factors; whole-plot vs. subplot error terms |
| `glmmTMB.ipynb` | Extended GLMMs via `glmmTMB`; zero-inflated and zero-truncated models; Beta, Tweedie, beta-binomial families; AR1 and spatial correlation structures |

**Key packages:** `lme4`, `lmerTest`, `broom.mixed`, `performance`, `pbkrtest`, `glmmTMB`, `DHARMa`, `emmeans`

---

## Dependencies

```r
install.packages(c("tidyverse", "lme4", "glmmTMB", "DHARMa", "performance",
                   "AICcmodavg", "MuMIn", "broom.mixed", "ggplot2"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
