# Mixed Effects Models

Notebooks covering linear and generalized linear mixed effects models (LMMs and GLMMs) in R. Mixed models account for non-independence in data arising from repeated measures, nested sampling designs, or hierarchical structure — common in both ecological fieldwork and industry datasets with grouped observations.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `lmm_basics.ipynb` | Linear mixed models with random intercepts and random slopes using `lme4` |
| `glmm_basics.ipynb` | Generalized linear mixed models for non-normal responses (binomial, Poisson, negative binomial) using `glmmTMB` |
| `random_effects_structure.ipynb` | Choosing and justifying random effects structure; crossed vs. nested random effects |
| `dharma_diagnostics.ipynb` | Residual diagnostics with `DHARMa`; overdispersion, zero-inflation, and model fit checks |
| `model_selection_lmm.ipynb` | AIC/AICc-based model selection and multi-model inference with `AICcmodavg` and `MuMIn` |

---

## Dependencies

```r
install.packages(c("tidyverse", "lme4", "glmmTMB", "DHARMa", "performance",
                   "AICcmodavg", "MuMIn", "broom.mixed", "ggplot2"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
