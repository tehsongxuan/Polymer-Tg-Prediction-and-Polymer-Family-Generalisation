
**Author:** Teh Song Xuan  
**Project:** Polymer_Tg_Project  
**Environment:** Python / Jupyter Notebook / Conda (`polymer-tg`)  
**Prediction target:** Reported glass-transition temperature, $T_g$ (°C)
**Prediction target:** Reported glass-transition temperature, T<sub>g</sub> (°C)

## View the Analysis

- [View the Jupyter notebook](TehSongXuan_Polymer_Tg_Project1.ipynb)
- [Open the HTML file page](TehSongXuan_Polymer_Tg_Project1.html) — select **Download raw file**, then open the downloaded HTML file in a web browser to view the formatted report.
- [Browse the supporting results](results/)

## Project Overview

This project develops a polymer-informatics workflow to predict reported glass-transition temperature from polymer repeat-unit structure and investigate whether the learned relationships transfer to unfamiliar polymer families.

The workflow covers dataset assessment, structural auditing, canonical-structure aggregation, RDKit descriptor generation, regression modelling, random structure-grouped validation, polymer-family holdout validation and structural-similarity diagnostics.

The central scientific question extends beyond obtaining a high $R^2$: **what happens to prediction performance when the model encounters a polymer family absent from training, and what evidence helps explain the deterioration?**
The central scientific question extends beyond obtaining a high R²: **what happens to prediction performance when the model encounters a polymer family absent from training, and what evidence helps explain the deterioration?**

The project connects experimental materials knowledge with Python-based data curation and machine learning. Its principal deliverable is a documented computational analysis of model generalisation and its limitations.

@@ -24,7 +30,7 @@ Glass-transition temperature describes the temperature region associated with a

Repeat-unit chemistry provides information about backbone rigidity, flexibility, aromaticity, steric effects and potential intermolecular interactions. However, a repeat-unit representation does not fully describe a manufactured or experimentally measured polymer sample.

Reported $T_g$ can also depend on molecular weight, tacticity, morphology, crosslinking, composition, processing history and measurement conditions. Consequently, this project predicts the dataset's reported values from the structural information available.
Reported T<sub>g</sub> can also depend on molecular weight, tacticity, morphology, crosslinking, composition, processing history and measurement conditions. Consequently, this project predicts the dataset's reported values from the structural information available.

For materials modelling, an overly optimistic validation result can encourage confidence in predictions for chemistry that the model has never learned. Evaluating transfer across polymer families therefore matters for assessing whether a model could support future materials screening.

@@ -60,8 +66,8 @@ The supplied working dataset contains **7,208 records** and four core fields. Fo
| Repeated canonical-structure groups | 31 |
| Additional occurrences consolidated | 34 |
| Eligible families for holdout validation | 11 |
| Structure-level reported $T_g$ range | −139 to 495 °C |
| Structure-level median reported $T_g$ | 134 °C |
| Structure-level reported T<sub>g</sub> range | −139 to 495 °C |
| Structure-level median reported T<sub>g</sub> | 134 °C |

### Data Source and Provenance

@@ -84,7 +90,7 @@ The structure count corresponds closely to the 7,174-polymer collection describe

### Target Variable

The target is **reported $T_g$ in °C**, making this a supervised regression problem. When multiple source records share a canonical structure, their median reported $T_g$ becomes the structure-level target. Source identifiers and disagreement information are retained.
The target is **reported T<sub>g</sub> in °C**, making this a supervised regression problem. When multiple source records share a canonical structure, the median of their supplied T<sub>g</sub> values becomes the structure-level target. Source identifiers and disagreement information are retained.

## Methodology

@@ -96,15 +102,15 @@ Fixed random-state settings support repeatable splitting and model fitting. The

### 2. Data Quality Assessment

The initial audit examines dataset dimensions, field completeness, record identifiers, SMILES uniqueness, parsing success and reported-$Tg$ distributions.
The initial audit examines dataset dimensions, field completeness, record identifiers, SMILES uniqueness, parsing success and reported T<sub>g</sub> distributions.

Record identity is distinguished from structural identity: different PIDs can describe the same encoded repeat unit. Treating these records as independent structures could give repeated inputs additional weight and allow structural overlap across validation partitions.

### 3. Structural Audit and Data Curation

RDKit canonicalisation produces **49 changes in written SMILES representation**, but no additional hidden duplicates beyond those already identified from the raw strings.

The audit finds **31 repeated canonical groups**, containing 65 source records. Of these groups, **28 have differing reported $T_g$ values**, with a maximum within-group range of **115 °C**.
The audit finds **31 repeated canonical groups**, containing 65 source records. Of these groups, **28 have differing reported T<sub>g</sub> values**, with a maximum within-group range of **115 °C**.

These disagreements are retained as traceable evidence. They may reflect missing sample or measurement information as well as possible source inconsistencies.

@@ -114,9 +120,9 @@ Connection markers are also reviewed: 7,204 source records have two connection p

Exploratory analysis examines:

- Reported-$T_g$ distributions before and after aggregation.
- Reported T<sub>g</sub> distributions before and after aggregation.
- Polymer-family representation and multi-label overlap.
- Within-family variation in reported $T_g$.
- Within-family variation in reported T<sub>g</sub>.
- Differences in family size and exclusive membership.
- Descriptor completeness, redundancy and numerical scale.

@@ -150,7 +156,7 @@ Related chemistry and members of the same polymer families may still appear in b

### 7. Preprocessing and Leakage Controls

Canonical aggregation prevents identical canonical inputs from crossing partitions. Identifiers and family labels are excluded from model inputs, and regression models are fitted only on the relevant training partition.
Canonical aggregation followed by structure-level splitting prevents identical canonical inputs from crossing partitions. Identifiers and family labels are excluded from model inputs, and regression models are fitted only on the relevant training partition.

**Preprocessing limitation:** non-finite, constant and exact duplicate descriptor filtering was performed using all 7,174 structures before splitting. Although the filtering did not use target values, it used descriptor information from future test structures. The evaluation therefore does not implement fully training-only preprocessing; its effect on the reported scores has not been quantified.

@@ -160,11 +166,11 @@ Canonical aggregation prevents identical canonical inputs from crossing partitio
|---|---|---|
| **MAE (°C)** | Average absolute prediction error; primary comparison metric | Lower |
| **RMSE (°C)** | Error measure that gives greater weight to large errors | Lower |
| **$R^2$** | Squared-error performance relative to predicting the evaluated test set's mean | Higher |
| **R²** | Squared-error performance relative to predicting the evaluated test set's mean | Higher |

An $R^2$ of 1 indicates perfect prediction; 0 matches the test-mean reference; a negative value is worse than that reference. The test mean is used to define this statistic, not supplied to the fitted model.
An R² of 1 indicates perfect prediction; 0 matches the test-mean reference; a negative value is worse than that reference. The test mean is used to define this statistic, not supplied to the fitted model.

Family-specific $R^2$ depends on the target variance within each test family. It is interpreted alongside MAE and RMSE rather than used alone to rank the severity of error.
Family-specific R² depends on the target variance within each test family. It is interpreted alongside MAE and RMSE rather than used alone to rank the severity of error.

### 9. Model Building and Baseline Comparison

@@ -177,7 +183,7 @@ Four tree-based regression models are evaluated using the same descriptor repres

A training-median baseline predicts **137 °C** for every Objective 1 test structure. This provides a reference without molecular information.

The analysis prioritises comparison across validation settings. Hyperparameter optimisation, model serialization and application deployment are not reported as completed components of this project.
The analysis prioritises comparison across validation settings. Hyperparameter optimisation, model serialisation and application deployment are not reported as completed components of this project.

### 10. Polymer-Family Holdout Validation

@@ -189,7 +195,7 @@ For each family:
2. Use exclusively labelled members of the held-out family as the test set.
3. Refit each regression model on the remaining training structures.
4. Confirm that the held-out family is absent from training.
5. Calculate MAE, RMSE and $R^2$.
5. Calculate MAE, RMSE and R².

This produces **44 family–model evaluations** and **2,552 held-out predictions per model**, or 10,208 predictions across four models. The four models predict the same collection of held-out test structures; these are not 10,208 distinct polymers.

@@ -200,7 +206,7 @@ For each held-out test structure, the maximum Morgan-fingerprint Tanimoto simila
The diagnostics compare structural similarity with absolute prediction error and examine family-level relationships involving:

- Mean nearest-training similarity.
- Absolute difference between test and training median $T_g$.
- Absolute difference between test and training median T<sub>g</sub>.
- Deviation of the test/training interquartile-range ratio from 1.
- Test-set size.

@@ -210,7 +216,7 @@ Pearson and Spearman correlations summarise these exploratory associations.

All four regression models outperform the training-median baseline.

| Model | MAE (°C) | RMSE (°C) | $R^2$ |
| Model | MAE (°C) | RMSE (°C) | R² |
|---|---:|---:|---:|
| **Extra Trees** | **25.196** | **37.092** | **0.886** |
| HistGradientBoosting | 25.657 | 37.426 | 0.884 |
@@ -220,15 +226,15 @@ All four regression models outperform the training-median baseline.

Extra Trees achieves the lowest observed Objective 1 MAE. Its advantage over HistGradientBoosting is small and has not been assessed across repeated splits, so it is described as the strongest model **in this evaluated random split**, rather than a universally superior predictor.

Its $R^2$ indicates approximately 88.6% lower squared error than the test-mean reference for this test population. The result supports useful structure–property information in the descriptors, while leaving transfer to unseen families to be tested separately.
Its R² indicates approximately 88.6% lower squared error than the test-mean reference for this test population. The result supports useful structure–property information in the descriptors, while leaving transfer to unseen families to be tested separately.

## Polymer-Family Holdout Results

### Extra Trees: Performance Across All 11 Families

The following results retain Extra Trees as a consistent reference from Objective 1. Each row represents a separately retrained model.

| Held-out family | Test structures | MAE (°C) | RMSE (°C) | $R^2$ |
| Held-out family | Test structures | MAE (°C) | RMSE (°C) | R² |
|---|---:|---:|---:|---:|
| Polycarbonates/thiocarbonates | 148 | 37.808 | 50.560 | 0.628 |
| Polyoxides/ethers/acetals | 298 | 38.813 | 52.955 | 0.668 |
@@ -246,9 +252,7 @@ The following results retain Extra Trees as a consistent reference from Objectiv

For each model and family, the deterioration ratio is:

$$
\text{MAE deterioration ratio} = \frac{\text{Family-holdout MAE}}{\text{Objective-1 MAE (all families)}}
$$
**MAE deterioration ratio = Family-holdout MAE ÷ Objective-1 MAE (all families)**

The family-level summary averages these four model-specific ratios. It is not a pooled prediction score or the ratio of two model-averaged MAEs.

@@ -274,7 +278,7 @@ All 11 ratios exceed 1. The comparison demonstrates higher family-holdout errors

At the individual-prediction level, higher nearest-training similarity is weakly associated with lower absolute error across all four models.

| Model | Predictions | Pearson $r$ | Spearman $\rho$ |
| Model | Predictions | Pearson r | Spearman ρ |
|---|---:|---:|---:|
| Decision Tree | 2,552 | −0.229 | −0.221 |
| Random Forest | 2,552 | −0.245 | −0.230 |
@@ -283,21 +287,21 @@ At the individual-prediction level, higher nearest-training similarity is weakly

These weak associations show considerable unexplained variation. Similarity is informative about structural coverage, but it does not determine an individual polymer's prediction error.

At the family level, mean nearest-training similarity has the strongest observed association with mean MAE deterioration among the examined factors: **Pearson $r = −0.640$** and **Spearman $\rho = −0.782$**.
At the family level, mean nearest-training similarity has the strongest observed association with mean MAE deterioration among the examined factors: **Pearson r = −0.640** and **Spearman ρ = −0.782**.

### Target-Distribution Shifts Also Matter

Absolute differences between training and test median $T_g$ are positively associated with family-level MAE deterioration: **Pearson $r = 0.516$** and **Spearman $\rho = 0.419$**.
Absolute differences between training and test median T<sub>g</sub> are positively associated with family-level MAE deterioration: **Pearson r = 0.516** and **Spearman ρ = 0.419**.

Polysiloxanes/silanes combine low mean nearest-training similarity (**0.363**) with a test median **143 °C below** the training median and the largest model-averaged MAE deterioration (**2.995×**).

Polyimides/thioimides also combine low similarity (**0.353**) with a large positive median shift (**157.45 °C**). These observations are consistent with difficulty transferring across structural and property domains.

### A Large Fall in $R^2$ Does Not Always Mean the Largest Absolute Error
### A Large Fall in R² Does Not Always Mean the Largest Absolute Error

Polyurethanes/thiourethanes have the largest model-averaged decline in $R^2$ (**−2.957**) but a smaller MAE deterioration ratio (**1.817×**) than Polysiloxanes/silanes.
Polyurethanes/thiourethanes have the largest model-averaged decline in R² (**mean ΔR² = −2.957**) but a smaller MAE deterioration ratio (**1.817×**) than Polysiloxanes/silanes.

Their test/training target IQR ratio is **0.223**, indicating a much narrower central target distribution. Since $R^2$ uses test-set variance as its reference, sizeable errors within a narrow target distribution can produce very negative values.
Their test/training target IQR ratio is **0.223**, indicating a much narrower central target distribution. Since R² uses test-set variance as its reference, sizeable errors within a narrow target distribution can produce very negative values.

### Model Choice Alone Does Not Resolve the Generalisation Gap

@@ -324,7 +328,7 @@ The findings support reduced structural coverage and target-distribution shift a
- Morgan fingerprints and Tanimoto similarity.
- Supervised regression and ensemble learning.
- Structure-aware splitting and family-level exclusion.
- MAE, RMSE and $R^2$ interpretation.
- MAE, RMSE and R² interpretation.
- Interpolation, chemical-domain transfer and applicability limits.
- Pearson and Spearman correlation.
- Target-distribution shift and evidence-based scientific interpretation.
@@ -333,7 +337,7 @@ The findings support reduced structural coverage and target-distribution shift a

### Joining Materials Experience with Analytics

This project connects my earlier composites and materials-characterisation background with Python-based analysis. It demonstrates how experimental context informs structural auditing, interpretation of conflicting reported values and recognition of information absent from a repeat-unit representation.
This project connects my earlier composites and materials-characterisation background with Python-based analysis. It illustrates how experimental context informs structural auditing, interpretation of conflicting reported values and recognition of information absent from a repeat-unit representation.

### Data Quality and Traceability

@@ -351,7 +355,7 @@ These capabilities are relevant to materials data curation, research analytics a

## Value of the Project

This project demonstrates my ability to:
The project brings together the following tasks:

- Translate a materials-science question into a computational study.
- Audit molecular records before model development.
@@ -374,28 +378,29 @@ This project demonstrates my ability to:
| Visualisation | Matplotlib |
| Machine learning | scikit-learn; Decision Tree, Random Forest, Extra Trees, HistGradientBoosting |
| Validation | Random structure-grouped split, polymer-family holdouts |
| Diagnostics | Tanimoto similarity, MAE, RMSE, $R^2$, Pearson and Spearman correlations |
| Diagnostics | Tanimoto similarity, MAE, RMSE, R², Pearson and Spearman correlations |
| Documentation | Notebook HTML export, GitHub Markdown |

## Project Files

| File | Purpose / status |
|---|---|
| `README.md` | GitHub project overview, methodology, results and interpretation |
| `results/` | Supporting CSV tables for family-holdout performance and explanatory analyses; see Supporting Results and Downloadable Tables below |
| `Polymer_Tg_Project1 (20).html` | Reviewed notebook export containing code, tables and scientific discussion |
| [`results/`](results/) | Supporting CSV tables for family-holdout performance and explanatory analyses; see Supporting Results and Downloadable Tables below |
| [`TehSongXuan_Polymer_Tg_Project1.html`](TehSongXuan_Polymer_Tg_Project1.html) | HTML notebook export containing code, tables and scientific discussion |
| [`TehSongXuan_Polymer_Tg_Project1.ipynb`](TehSongXuan_Polymer_Tg_Project1.ipynb) | Editable Jupyter notebook with saved outputs |
| `Tg_SMILES_class_pid_polyinfo_median (1).csv` | Source-data filename recorded in the notebook; not bundled with this README |
| `data/processed/Tg_structure_level_processed_v1.csv` | Structure-level data export documented in the notebook; not bundled with this README |

The HTML export can be downloaded and opened in a browser. Running the analysis requires the original `.ipynb` notebook, its input files and a compatible environment; the HTML export itself is not executable.
The HTML export can be downloaded and opened in a browser. Running the analysis requires the original `.ipynb` notebook, its input files and a compatible environment; the HTML export itself is not executable. The notebook uses paths such as `../data/raw/` and `../results/`, which assume execution from a notebook subfolder. When running it from the repository root, adjust these paths or recreate the expected folder layout.

Dataset redistribution remains subject to the source's applicable terms. Inclusion in this file inventory does not establish that a dataset is available for public redistribution.

## Project Direction and Review Status
## Project Direction

The study follows the requested scientific direction: use polymer-property data, generate RDKit descriptors, predict $T_g$, compare random validation with polymer-class holdouts and explain the deterioration.
The project connects earlier composites and materials-characterisation experience with Python-based data analysis and machine learning. It uses polymer-property data and RDKit descriptors to predict glass-transition temperature, then compares random structure-grouped validation with polymer-family holdouts.

The emphasis is on connecting materials knowledge with data curation, validation and workflow engineering. No assessment, endorsement or approval by an external reviewer is claimed; the direction provided before the study is distinct from a review of its completed results.
The central aim is to investigate where predictive performance deteriorates and explain the observed patterns using structural coverage, property-distribution shifts and the limitations of repeat-unit representations. This places scientific interpretation alongside model scores and develops practical foundations for materials data curation and workflow engineering.

## Supporting Results and Downloadable Tables

@@ -424,9 +429,9 @@ These tables support the notebook’s comparison of random structure-grouped val

## Conclusion

The curated dataset supports strong prediction under random structure-grouped validation: Extra Trees achieves an MAE of **25.196 °C**, RMSE of **37.092 °C** and $R^2$ of **0.886**.
The curated dataset supports strong prediction under random structure-grouped validation: Extra Trees achieves an MAE of **25.196 °C**, RMSE of **37.092 °C** and R² of **0.886**.

Performance deteriorates when polymer families are excluded from training. Across 11 families, model-averaged MAE deterioration ratios range from **1.447× to 2.995×** relative to each model's overall random-validation reference. Several holdouts produce negative $R^2$ values.
Performance deteriorates when polymer families are excluded from training. Across 11 families, model-averaged MAE deterioration ratios range from **1.447× to 2.995×** relative to each model's overall random-validation reference. Several holdouts produce negative R² values.

Structural coverage and target-distribution shifts provide plausible, exploratory explanations for this gap, while missing polymer and experimental information limits what the representations can capture.

@@ -442,4 +447,3 @@ The principal contribution is a traceable demonstration that **successful predic
**Teh Song Xuan**  
**GitHub:** [tehsongxuan](https://github.com/tehsongxuan)  
**Portfolio areas:** Materials Informatics, Data Curation, Statistical Analysis, Machine Learning and Research Workflow Engineering
