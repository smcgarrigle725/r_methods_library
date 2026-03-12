# r_methods_library

**Owner:** Samantha McGarrigle  
**Purpose:** Comprehensive statistical methods reference library in R for portfolio and interview preparation. Targets data science and data engineering roles in healthcare, finance, insurance, and ecology.

---

## Folder Structure

| # | Folder | Notebooks | Primary Packages | Theme |
|---|---|---|---|---|
| 01 | `01_basic_inference` | 6 | base R, rstatix, effectsize, pwr, emmeans, multcomp | Ecological / Mixed |
| 02 | `02_regression` | 12 | tidyverse, car, MASS, glmnet, smatr, VGAM | Ecological / Mixed |
| 03 | `03_mixed_effects_models` | 9 | lme4, lmerTest, DHARMa, glmmTMB, emmeans | Ecological |
| 04 | `04_gams` | 6 | mgcv, gratia, ggplot2 | Ecological |
| 05 | `05_multivariate` | 13 | vegan, ade4, indicspecies, MASS, CCA, MVN | Ecological |
| 06 | `06_nonparametric` | 5 | coin, NSM3, rstatix | Mixed |
| 07 | `07_time_series` | 10 | forecast, tseries, prophet, TSA | Mixed |
| 08 | `08_survival_analysis` | 6 | survival, survminer, cmprsk | Clinical / Healthcare |
| 09 | `09_bayesian_methods` | 8 | brms, rstanarm, bayesplot, priorsense, metafor | Mixed |
| 10 | `10_classification` | 8 | tidymodels, ranger, xgboost, kernlab | Mixed |
| 11 | `11_cross_validation_model_selection` | 8 | tidymodels, caret, rsample | Mixed |
| 12 | `12_clustering` | 7 | cluster, factoextra, mclust | Ecological / Mixed |
| 13 | `13_dimensionality_reduction` | 7 | vegan, FactoMineR, Rtsne, umap | Ecological |
| 14 | `14_model_diagnostics_interpretation` | 13 | DHARMa, car, DALEX, iml, shapr, geepack | Mixed |
| 15 | `15_ab_testing_experimental_design` | 9 | pwr, lmerTest, BayesFactor | Mixed |
| **Total** | | **~127 notebooks** | | |

---

## Notebook Standards

- **Format:** Jupyter notebooks (`.ipynb`), R kernel via IRkernel
- **Structure:** Overview → setup / data simulation → topic sections with code → Common Pitfalls section → footer
- **Footer:** `*r_methods_library - Samantha McGarrigle*`
- **Data:** Simulated inline where possible; uses built-in R datasets (iris, mtcars, etc.) otherwise — no downloads required
- **Pitfalls:** Minimum 6 concrete pitfalls per notebook
- **Style:** tidyverse-first where appropriate; base R shown for comparison

## Folder Standards

- Every folder has a `README.md` covering: purpose, notebook list with topics, key packages, run instructions

### IRkernel Setup

```r
install.packages('IRkernel')
IRkernel::installspec()   # registers the R kernel with Jupyter
```

Then launch Jupyter and select "R" as the kernel.

---

## Notebook Detail by Folder

### 01 basic_inference ✅ COMPLETE
1. `t_tests` — One-sample, independent (Welch's & Student's), and paired t-tests; effect sizes (Cohen's d)
2. `anova` — One-way and two-way ANOVA, Tukey HSD / Bonferroni post-hoc, assumption checking
3. `chi_square_fisher` — Chi-square test of independence, goodness-of-fit, Fisher's exact test for small samples
4. `confidence_intervals_effect_sizes` — CI construction, Cohen's d, eta-squared, power analysis with pwr
5. `transformations` — sqrt, log, arcsine, and Box-Cox transformations; when and why to transform; back-transforming estimates and CIs
6. `multiple_comparisons` — Tukey HSD, Bonferroni, Dunnett, and Holm corrections; planned (a priori) vs. unplanned (a posteriori) contrasts; experiment-wise Type I error control

### 02 regression ✅ COMPLETE
1. `linear_regression` — OLS, assumptions, diagnostics, interpretation, transformations
2. `logistic_regression` — Binary logistic, odds ratios, ROC/AUC, Hosmer-Lemeshow
3. `multinomial_regression` — Multinomial logistic regression with nnet/VGAM, relative risk ratios
4. `ordinal_regression` — Proportional odds model with MASS::polr, parallel lines assumption
5. `glm_count_data` — Poisson, negative binomial, zero-inflated models for count outcomes
6. `regularized_regression` — Ridge, LASSO, elastic net with glmnet; cross-validated lambda selection
7. `regression_diagnostics` — Residual plots, Cook's distance, VIF, leverage, influential observations
8. `ancova` — ANCOVA as regression with continuous covariate + factor; homogeneity of slopes; adjusted means; when ANCOVA vs factorial ANOVA
9. `model2_regression` — Model II regression (major axis, standardised major axis / RMA); when X is also measured with error; morphometrics and allometry
10. `weighted_least_squares` — Weighted least squares for heteroscedastic data; known-variance weights; survey weights
11. `log_linear_models` — Log-linear models for multi-way contingency tables; model selection beyond chi-square; 3-way tables
12. `smoothing` — LOESS/LOWESS, regression splines, and kernel smoothing as standalone tools; distinct from GAMs

### 03 mixed_effects_models ✅ COMPLETE
1. `lmm_basics` — Linear mixed models with lme4, random intercepts vs slopes, REML vs ML
2. `glmm_basics` — GLMMs for binary and count outcomes, link functions, random effects in GLMMs
3. `random_effects_structure` — Maximal vs minimal random effects, nested vs crossed designs, convergence
4. `model_selection_lmm` — AIC/BIC comparison, LRT, anova() for fixed effects testing
5. `dharma_diagnostics` — Simulation-based residuals with DHARMa, uniformity, dispersion, zero-inflation tests
6. `rcb_designs` — Randomised complete block designs; blocking rationale; Latin squares; Tukey's test for non-additivity
7. `repeated_measures_anova` — Classical repeated measures ANOVA; Mauchly's sphericity test; Greenhouse-Geisser and Huynh-Feldt corrections; contrast with LMM approach
8. `split_plot_designs` — Split-plot (partly nested) designs; between- and within-subjects factors; whole-plot vs. subplot error terms
9. `glmmTMB` — Extended GLMMs via glmmTMB; zero-inflated and zero-truncated models; Beta, Tweedie, beta-binomial families; AR1 and spatial correlation structures

### 04 gams ✅ COMPLETE
1. `gam_basics` — mgcv::gam(), smooth terms s(), basis functions, effective degrees of freedom
2. `gam_families` — Gaussian, binomial, Poisson, negative binomial, Tweedie, Gamma families
3. `gam_interactions` — Tensor products te()/ti(), factor-smooth interactions, spatial smooths with s(x,y)
4. `gam_diagnostics` — gam.check(), k-index, concurvity, gratia::appraise()
5. `gam_visualization` — plot.gam(), gratia::draw(), partial effects, gratia::smooth_estimates()
6. `gam_vs_glm` — When to use GAM vs GLM, AIC comparison, partial vs full non-linearity

### 05 multivariate ✅ COMPLETE
1. `multivariate_assumptions` — Multivariate normality, homogeneity of dispersions (betadisper), distance choices
2. `pca` — PCA on environmental and species data, scree plots, biplots, interpretation
3. `nmds` — Non-metric MDS with vegan, stress diagnostics, envfit vectors, ggplot2 biplots
4. `permanova` — adonis2(), pairwise tests, restricted permutations (permute), interaction testing
5. `anosim_mantel` — ANOSIM vs PERMANOVA comparison, Mantel and partial Mantel tests, spatial autocorrelation
6. `dbrda` — Distance-based RDA, forward selection, variance partitioning with varpart()
7. `beta_diversity` — Beta diversity decomposition into turnover and nestedness (betapart)
8. `indicator_species` — IndVal with indicspecies, A-B component plots, multi-level patterns
9. `biplots_visualization` — Publication-quality ordination plots with ggplot2, site scores, hulls, centroids
10. `manova` — MANOVA; Pillai, Wilks, Hotelling-Lawley, Roy statistics; follow-up univariate tests; canonical discriminant scores
11. `discriminant_analysis` — LDA and QDA for group separation and classification; structure matrix; LOO-CV accuracy
12. `rda` — Redundancy analysis (linear constrained ordination); Hellinger-transformed species data; variance partitioning; forward selection
13. `canonical_correlation` — CCorA relating two continuous variable sets; canonical loadings; redundancy index

### 06 nonparametric ✅ COMPLETE
1. `rank_tests_two_groups` — Mann-Whitney U, Wilcoxon signed-rank, stochastic superiority interpretation
2. `rank_tests_multiple_groups` — Kruskal-Wallis, Dunn post-hoc, Friedman test for repeated measures
3. `correlation_nonparametric` — Spearman and Kendall correlation, ties handling, confidence intervals
4. `permutation_tests` — Permutation test framework, custom test statistics, from-scratch implementation
5. `normality_tests` — Shapiro-Wilk, KS test, Q-Q plots, sample size sensitivity demonstration

### 07 time_series ✅ COMPLETE
1. `stationarity` — ADF and KPSS tests, unit roots, differencing strategies, KPSS vs ADF interpretation
2. `decomposition` — Classical decomposition, STL, trend/seasonal/remainder extraction
3. `acf_pacf` — ACF and PACF interpretation, identifying ARIMA orders, seasonal patterns
4. `arima` — ARIMA model fitting, auto.arima(), manual identification, residual diagnostics
5. `sarima` — Seasonal ARIMA, seasonal differencing, SARIMA order selection
6. `exponential_smoothing` — SES, Holt's linear trend, Holt-Winters, ETS framework with forecast
7. `prophet_forecasting` — Meta Prophet in R, trend changepoints, holiday effects, cross-validation
8. `intervention_analysis` — Interrupted time series, ARIMA with intervention terms, TSA package
9. `ts_regression` — Dynamic regression, regression with ARIMA errors, ARIMAX, external regressors
10. `ts_cross_validation` — Rolling-origin evaluation, tsCV(), MASE/RMSE/MAE comparison

### 08 survival_analysis ✅ COMPLETE
1. `kaplan_meier` — Survfit, KM curves, log-rank test, strata comparison, ggsurvplot
2. `cox_proportional_hazards` — coxph(), hazard ratios, Schoenfeld residuals, PH assumption testing
3. `aft_models` — Accelerated failure time models (survreg), Weibull / log-normal / log-logistic distributions
4. `survival_visualization` — Forest plots, cumulative hazard, landmark analysis, restricted mean survival
5. `competing_risks` — cmprsk::cuminc(), Fine-Gray subdistribution hazards, cause-specific vs subdistribution
6. `time_varying_covariates` — tmerge(), episode splitting, time-dependent predictors in Cox models

### 09 bayesian_methods ✅ COMPLETE
1. `bayesian_fundamentals` — Prior, likelihood, posterior, Bayes theorem, conjugate pairs
2. `bayesian_regression_brms` — brms model syntax, prior specification, MCMC sampling, posterior summaries
3. `hierarchical_models` — Partial pooling, multilevel priors, random effects as Bayesian hierarchy
4. `mcmc_diagnostics` — R-hat, effective sample size, trace plots, posterior predictive checks with bayesplot
5. `model_comparison_waic` — WAIC, LOO-CV with loo package, stacking, model weights
6. `prior_sensitivity` — Sensitivity analysis to prior choice, priorsense, weakly informative vs informative
7. `bayesian_workflow` — Simulation-based calibration, prior predictive checks, iterative model building
8. `meta_analysis` — Combining results across studies; fixed vs. random effects; forest plots; heterogeneity (I²); funnel plots; Bayesian meta-analysis via brms and metafor

### 10 classification ✅ COMPLETE
1. `logistic_regression_classification` — Binary and multiclass logistic with tidymodels, confusion matrix, ROC
2. `decision_trees` — rpart trees, pruning, cp selection, variable importance, tree visualization
3. `random_forest` — ranger::ranger(), OOB error, variable importance (impurity vs permutation)
4. `gradient_boosting` — xgboost in R, hyperparameter tuning, early stopping, SHAP values
5. `model_evaluation` — Confusion matrix, precision/recall/F1, ROC-AUC, calibration curves, tidymodels metrics
6. `imbalanced_data` — SMOTE (themis), class weights, threshold tuning, imbalanced performance metrics
7. `shap_explainability` — shapr, SHAP summary plots, dependence plots, interaction effects
8. `svm_classification` — kernlab::ksvm(), kernel selection, cost/gamma tuning, SVM vs tree comparison

### 11 cross_validation_model_selection ✅ COMPLETE
1. `train_test_split` — rsample::initial_split(), stratified splits, data leakage prevention
2. `kfold_cv` — vfold_cv(), repeated k-fold, tune_grid(), collect_metrics()
3. `loocv` — Leave-one-out CV with tidymodels, when LOOCV is appropriate, computational cost
4. `ts_cv` — Time series CV with rsample::rolling_origin(), respecting temporal order
5. `hyperparameter_tuning` — tune_grid(), tune_bayes(), racing methods, optimal hyperparameter selection
6. `aic_model_selection` — AIC, BIC, stepwise selection, model comparison with ANOVA for nested models
7. `nested_cv` — Nested cross-validation for unbiased performance estimation, outer/inner loop structure
8. `bootstrap_resampling` — rsample::bootstraps(), bootstrap CIs, .632 estimator, parameter uncertainty

### 12 clustering ✅ COMPLETE
1. `kmeans` — stats::kmeans(), elbow method, silhouette, within-cluster SS, cluster stability
2. `hierarchical_clustering` — hclust(), linkage methods (Ward, complete, average), dendrograms, cutree()
3. `dbscan` — dbscan::dbscan(), epsilon/minPts tuning, noise points, cluster shape flexibility
4. `gaussian_mixture_models` — mclust::Mclust(), BIC model selection, covariance structure, soft assignments
5. `cluster_validation` — Internal (silhouette, CH index) vs external (ARI, NMI) validation metrics
6. `dimensionality_reduction_overview` — PCA/t-SNE/UMAP before clustering, distance choice, scaling importance
7. `cluster_profiling` — Characterising clusters with means, visualisations, heatmaps, reporting results

### 13 dimensionality_reduction ✅ COMPLETE
1. `pca` — prcomp(), scree plots, loadings, biplots, proportion of variance explained
2. `factor_analysis` — Exploratory FA with psych, factor rotation (varimax/oblimin), communalities
3. `tsne` — Rtsne::Rtsne(), perplexity tuning, reproducibility, t-SNE pitfalls and interpretation
4. `umap` — umap::umap(), n_neighbors/min_dist parameters, UMAP vs t-SNE comparison
5. `correspondence_analysis` — ca package, contingency tables, symmetric vs asymmetric biplots
6. `nmds` — metaMDS() from vegan, Bray-Curtis distances, species/site scores, stress interpretation
7. `sparse_methods` — Sparse PCA (sparsepca), NMF (NMF package), interpretable low-rank decompositions

### 14 model_diagnostics_interpretation ✅ COMPLETE
1. `residual_diagnostics` — Residual plots, scale-location, QQ, residuals vs leverage, base R and ggplot2
2. `dharma_diagnostics` — Simulation-based diagnostics for GLMMs, dispersion tests, zero-inflation
3. `multicollinearity` — VIF, condition numbers, tolerance, ridge regression as remedy
4. `influential_observations` — Cook's distance, DFBETAS, hat matrix, leverage vs influence distinction
5. `overdispersion` — Detecting overdispersion, quasi-families, negative binomial alternatives
6. `model_comparison` — AIC/BIC tables, LRT for nested models, cross-validation comparison
7. `shap_values` — DALEX / shapr SHAP values, shapley decomposition, interaction effects
8. `partial_dependence` — Partial dependence plots with iml, marginal effects, feature interaction H-statistic
9. `permutation_importance` — Model-agnostic permutation importance with iml, stability across random seeds
10. `accumulated_local_effects` — ALE plots vs PDPs, avoiding extrapolation, iml::FeatureEffect()
11. `pseudoreplication` — Hurlbert (1984) pseudoreplication taxonomy; true replication vs. subsampling; interspersion; ICC-based detection; design audit checklist
12. `gee` — Generalised Estimating Equations; working correlation structures; marginal vs. subject-specific interpretation; comparison with mixed models
13. `results_presentation` — SD vs. SE vs. 95% CI for error bars; publication-quality figures with raw data; ANOVA and regression table reporting; mixed model write-up standards

### 15 ab_testing_experimental_design ✅ COMPLETE
1. `power_analysis` — pwr package, t-test / ANOVA / proportion test power, sample size curves
2. `ab_test_fundamentals` — Two-proportion z-test, t-test for means, one-sided vs two-sided, p-values vs CIs
3. `multiple_testing_correction` — Bonferroni, Holm, Benjamini-Hochberg FDR, p.adjust(), when each applies
4. `experiment_design_principles` — Randomisation, blocking, factorial designs, confounding, CONSORT
5. `sequential_testing` — Group sequential designs, alpha spending, O'Brien-Fleming boundaries
6. `minimum_detectable_effect` — MDE calculation, practical vs statistical significance, effect size framing
7. `bayesian_ab_testing` — BayesFactor package, Bayes factors, posterior probability of superiority
8. `factorial_designs` — 2^k designs, interaction effects, ANOVA for factorial experiments
9. `regression_discontinuity` — Sharp and fuzzy RD designs, bandwidth selection, rdrobust package

---

## Build Status

| Folder | Status |
|---|---|
| 01_basic_inference | ✅ Complete |
| 02_regression | ✅ Complete |
| 03_mixed_effects_models | ✅ Complete |
| 04_gams | ✅ Complete |
| 05_multivariate | ✅ Complete |
| 06_nonparametric | ✅ Complete |
| 07_time_series | ✅ Complete |
| 08_survival_analysis | ✅ Complete |
| 09_bayesian_methods | ✅ Complete |
| 10_classification | ✅ Complete |
| 11_cross_validation_model_selection | ✅ Complete |
| 12_clustering | ✅ Complete |
| 13_dimensionality_reduction | ✅ Complete |
| 14_model_diagnostics_interpretation | ✅ Complete |
| 15_ab_testing_experimental_design | ✅ Complete |

---
*r_methods_library - Samantha McGarrigle*
