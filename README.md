# LLM Anna Karenina

Code repository for the preregistered project **Do LLMs Preserve Gradients in Human Heterogeneity?**

The project examines whether large language models substantially compress human well-being variation while preserving its socioeconomic structure, using Wave 7 of the World Values Survey.

## Notebooks

- `notebooks/1_WVS_prepare_FINAL_REVISED.ipynb` — frozen data-preparation pipeline used to construct respondent profiles for prediction.
- `notebooks/2_WVS_predict_FINAL_REVISED.ipynb` — frozen LLM prediction pipeline.
- `notebooks/3_WVS_Human_LLM_Analysis.ipynb` — Human + LLM analysis, including raw and normalized income-dispersion profiles, bootstrap inference, weighting robustness, country fixed-effects analyses, country-level gradient analyses, and RIF-Oaxaca decompositions.
- `notebooks/5_WVS_OLS_Lasso_NonLLM_Benchmark.ipynb` — post-preregistration OLS/Lasso benchmark using the same respondent information supplied to the LLMs. It uses five-fold out-of-sample prediction, nested Lasso tuning, normalized income-dispersion comparisons, and a 200-replication country-cluster bootstrap.

The analysis notebooks are committed without stored execution outputs to keep the repository lightweight and reproducible; running the notebooks regenerates the reported outputs.
