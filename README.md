[TehSongXuan_Polymer_Tg_Project1.html](https://github.com/user-attachments/files/31931429/TehSongXuan_Polymer_Tg_Project1.html)
# Polymer Glass-Transition Temperature Prediction and Polymer-Family Generalisation

### A Materials-Informatics Machine Learning Workflow for Data Curation, Molecular Representation and Chemistry-Aware Validation

**Author:** Teh Song Xuan  
**Project:** Polymer_Tg_Project  
**Environment:** Python / Jupyter Notebook / Conda (`polymer-tg`)  
**Prediction target:** Reported glass-transition temperature, T<sub>g</sub> (°C)

## View the Analysis

- [View the Jupyter notebook](TehSongXuan_Polymer_Tg_Project1.ipynb)
- [Open the HTML file page](TehSongXuan_Polymer_Tg_Project1.html) — select **Download raw file**, then open the downloaded HTML file in a web browser to view the formatted report.
- [Browse the supporting results](results/)

## Project Overview

This project develops a polymer-informatics workflow to predict reported glass-transition temperature from polymer repeat-unit structure and investigate whether the learned relationships transfer to unfamiliar polymer families.

The workflow covers dataset assessment, structural auditing, canonical-structure aggregation, RDKit descriptor generation, regression modelling, random structure-grouped validation, polymer-family holdout validation and structural-similarity diagnostics.

The central scientific question extends beyond obtaining a high R²: **what happens to prediction performance when the model encounters a polymer family absent from training, and what evidence helps explain the deterioration?**

The project connects experimental materials knowledge with Python-based data curation and machine learning. Its principal deliverable is a documented computational analysis of model generalisation and its limitations.

## Scientific Context

Glass-transition temperature describes the temperature region associated with a substantial change in segmental mobility in the amorphous portion of a polymer. It is relevant to understanding material behaviour across operating temperatures.

Repeat-unit chemistry provides information about backbone rigidity, flexibility, aromaticity, steric effects and potential intermolecular interactions. However, a repeat-unit representation does not fully describe a manufactured or experimentally measured polymer sample.

Reported T<sub>g</sub> can also depend on molecular weight, tacticity, morphology, crosslinking, composition, processing history and measurement conditions. Consequently, this project predicts the dataset's reported values from the structural information available.

For materials modelling, an overly optimistic validation result can encourage confidence in predictions for chemistry that the model has never learned. Evaluating transfer across polymer families therefore matters for assessing whether a model could support future materials screening.

## Project Objectives

The project aims to:

- Assess polymer-data quality, provenance and structural identity.
- Construct one traceable modelling record per canonical repeat-unit structure.
- Generate and audit RDKit molecular descriptors and Morgan fingerprints.
- Compare four regression models against a structure-blind baseline.
- Evaluate prediction under random structure-grouped validation.
- Test generalisation by excluding entire polymer families from training.
- Examine structural similarity and target-distribution shifts as possible explanations for performance deterioration.
- Communicate the results with appropriate scientific limitations.

| Validation objective | Question addressed |
|---|---|
| **Objective 1 — Random structure-grouped validation** | Can the models predict unseen structures within broadly represented polymer chemistry? |
| **Objective 2 — Polymer-family holdout validation** | Can the models predict exclusively labelled members of a family completely excluded from training? |

## Dataset

The supplied working dataset contains **7,208 records** and four core fields. Following canonical-structure aggregation, the modelling dataset contains **7,174 unique canonical repeat-unit representations**.

| Dataset characteristic | Result |
|---|---:|
| Source records | 7,208 |
| Unique raw SMILES | 7,174 |
| Unique canonical SMILES | 7,174 |
| Missing values in the four supplied fields | 0 |
| RDKit parsing failures | 0 |
| Repeated canonical-structure groups | 31 |
| Additional occurrences consolidated | 34 |
| Eligible families for holdout validation | 11 |
| Structure-level reported T<sub>g</sub> range | −139 to 495 °C |
| Structure-level median reported T<sub>g</sub> | 134 °C |

### Data Source and Provenance

The local source file is `Tg_SMILES_class_pid_polyinfo_median (1).csv`. The notebook identifies the dataset page [Tg SMILES | PID | PolyInfo Class](https://www.kaggle.com/datasets/fridaycode/tg-smiles-pid-polyinfo-class).

The file is treated as a **third-party, PoLyInfo-related processed dataset**, rather than an official PoLyInfo export. Equivalence between the local copy and the currently hosted file has not been independently verified.

The structure count corresponds closely to the 7,174-polymer collection described by Uddin and Fan (2024). That correspondence does not establish that the paper's authors created or used this exact PID- and family-enriched file.

### Data Dictionary

| Variable | Description | Use in this project |
|---|---|---|
| `SMILES` | Encoded polymer repeat-unit structure, including connection markers | Structural auditing, canonicalisation, descriptors and fingerprints |
| `Tg` | Reported glass-transition temperature in °C | Continuous regression target |
| `Polymer Class` | One or more polymer-family labels | Family analysis and holdout construction |
| `PID` | Source record identifier | Traceability and audit investigation |

`PID` and `Polymer Class` are excluded from the predictive molecular features.

### Target Variable

The target is **reported T<sub>g</sub> in °C**, making this a supervised regression problem. When multiple source records share a canonical structure, the median of their supplied T<sub>g</sub> values becomes the structure-level target. Source identifiers and disagreement information are retained.

## Methodology

### 1. Environment Setup

The analysis uses Python in a Jupyter Notebook with the Conda environment `polymer-tg`. Core libraries include RDKit, pandas, NumPy, Matplotlib and scikit-learn.

Fixed random-state settings support repeatable splitting and model fitting. The notebook documents the processing decisions, numerical checks and validation results.

### 2. Data Quality Assessment

The initial audit examines dataset dimensions, field completeness, record identifiers, SMILES uniqueness, parsing success and reported T<sub>g</sub> distributions.

Record identity is distinguished from structural identity: different PIDs can describe the same encoded repeat unit. Treating these records as independent structures could give repeated inputs additional weight and allow structural overlap across validation partitions.

### 3. Structural Audit and Data Curation

RDKit canonicalisation produces **49 changes in written SMILES representation**, but no additional hidden duplicates beyond those already identified from the raw strings.

The audit finds **31 repeated canonical groups**, containing 65 source records. Of these groups, **28 have differing reported T<sub>g</sub> values**, with a maximum within-group range of **115 °C**.

These disagreements are retained as traceable evidence. They may reflect missing sample or measurement information as well as possible source inconsistencies.

Connection markers are also reviewed: 7,204 source records have two connection points, three have three, and one has four. Unusual structures are flagged and retained rather than automatically rejected.

### 4. Exploratory Data Analysis

Exploratory analysis examines:

- Reported T<sub>g</sub> distributions before and after aggregation.
- Polymer-family representation and multi-label overlap.
- Within-family variation in reported T<sub>g</sub>.
- Differences in family size and exclusive membership.
- Descriptor completeness, redundancy and numerical scale.

Aggregation preserves the dataset's broad target distribution. Family labels overlap substantially, making explicit multi-label handling necessary for holdout validation.

### 5. Molecular Feature Engineering

The canonical repeat-unit graphs are converted into **217 initial RDKit descriptors**. Descriptor curation removes:

- 12 columns containing missing or infinite values.
- 11 constant columns.
- Eight exact duplicate columns.

The raw `Ipc` descriptor is replaced by `log10(Ipc)` to reduce its extreme numerical range. This transformation does not change the descriptor count or remove structures; the audit does not establish that it improves predictive accuracy.

The final matrix contains **7,174 structures × 186 descriptors**, with no missing or infinite values and preserved alignment to the target table.

**Morgan fingerprints** are generated separately using radius 2 and 2,048 bits. The regression models use the RDKit descriptors; fingerprints support the structural-similarity analysis.

### 6. Random Structure-Grouped Train–Test Split

Objective 1 uses an 80:20 split with random seed 42.

| Split characteristic | Result |
|---|---:|
| Training structures | 5,739 |
| Test structures | 1,435 |
| Canonical-structure overlap | 0 |

Related chemistry and members of the same polymer families may still appear in both partitions. This evaluation therefore measures prediction within broadly familiar chemical space.

### 7. Preprocessing and Leakage Controls

Canonical aggregation followed by structure-level splitting prevents identical canonical inputs from crossing partitions. Identifiers and family labels are excluded from model inputs, and regression models are fitted only on the relevant training partition.

**Preprocessing limitation:** non-finite, constant and exact duplicate descriptor filtering was performed using all 7,174 structures before splitting. Although the filtering did not use target values, it used descriptor information from future test structures. The evaluation therefore does not implement fully training-only preprocessing; its effect on the reported scores has not been quantified.

### 8. Model Evaluation Criteria

| Metric | Interpretation | Preferred direction |
|---|---|---|
| **MAE (°C)** | Average absolute prediction error; primary comparison metric | Lower |
| **RMSE (°C)** | Error measure that gives greater weight to large errors | Lower |
| **R²** | Squared-error performance relative to predicting the evaluated test set's mean | Higher |

An R² of 1 indicates perfect prediction; 0 matches the test-mean reference; a negative value is worse than that reference. The test mean is used to define this statistic, not supplied to the fitted model.

Family-specific R² depends on the target variance within each test family. It is interpreted alongside MAE and RMSE rather than used alone to rank the severity of error.

### 9. Model Building and Baseline Comparison

Four tree-based regression models are evaluated using the same descriptor representation:

- Decision Tree Regressor.
- Random Forest Regressor.
- Extra Trees Regressor.
- HistGradientBoosting Regressor.

A training-median baseline predicts **137 °C** for every Objective 1 test structure. This provides a reference without molecular information.

The analysis prioritises comparison across validation settings. Hyperparameter optimisation, model serialisation and application deployment are not reported as completed components of this project.

### 10. Polymer-Family Holdout Validation

A family is eligible when it has at least **100 total labelled structures** and **50 exclusively labelled structures**. Eleven families meet both thresholds.

For each family:

1. Remove every structure carrying that family label from training, including multi-label structures.
2. Use exclusively labelled members of the held-out family as the test set.
3. Refit each regression model on the remaining training structures.
4. Confirm that the held-out family is absent from training.
5. Calculate MAE, RMSE and R².

This produces **44 family–model evaluations** and **2,552 held-out predictions per model**, or 10,208 predictions across four models. The four models predict the same collection of held-out test structures; these are not 10,208 distinct polymers.

### 11. Structural-Similarity and Distribution-Shift Diagnostics

For each held-out test structure, the maximum Morgan-fingerprint Tanimoto similarity to the corresponding training set is calculated. This represents its nearest available structural analogue under the selected fingerprint representation.

The diagnostics compare structural similarity with absolute prediction error and examine family-level relationships involving:

- Mean nearest-training similarity.
- Absolute difference between test and training median T<sub>g</sub>.
- Deviation of the test/training interquartile-range ratio from 1.
- Test-set size.

Pearson and Spearman correlations summarise these exploratory associations.

## Model Comparison and Final Random-Validation Performance

All four regression models outperform the training-median baseline.

| Model | MAE (°C) | RMSE (°C) | R² |
|---|---:|---:|---:|
| **Extra Trees** | **25.196** | **37.092** | **0.886** |
| HistGradientBoosting | 25.657 | 37.426 | 0.884 |
| Random Forest | 27.477 | 39.646 | 0.870 |
| Decision Tree | 39.740 | 59.221 | 0.709 |
| Training-median baseline | 92.916 | 109.875 | ≈ 0 |

Extra Trees achieves the lowest observed Objective 1 MAE. Its advantage over HistGradientBoosting is small and has not been assessed across repeated splits, so it is described as the strongest model **in this evaluated random split**, rather than a universally superior predictor.

Its R² indicates approximately 88.6% lower squared error than the test-mean reference for this test population. The result supports useful structure–property information in the descriptors, while leaving transfer to unseen families to be tested separately.

## Polymer-Family Holdout Results

### Extra Trees: Performance Across All 11 Families

The following results retain Extra Trees as a consistent reference from Objective 1. Each row represents a separately retrained model.

| Held-out family | Test structures | MAE (°C) | RMSE (°C) | R² |
|---|---:|---:|---:|---:|
| Polycarbonates/thiocarbonates | 148 | 37.808 | 50.560 | 0.628 |
| Polyoxides/ethers/acetals | 298 | 38.813 | 52.955 | 0.668 |
| Polyesters/thioesters | 424 | 40.487 | 52.001 | 0.686 |
| Polyphenylenes | 100 | 45.639 | 64.165 | 0.324 |
| Polysulfides | 85 | 52.826 | 67.146 | 0.258 |
| Polyimines | 216 | 52.967 | 72.280 | 0.673 |
| Polyvinyls | 241 | 53.105 | 73.524 | 0.072 |
| Polyurethanes/thiourethanes | 76 | 53.546 | 69.854 | −1.918 |
| Polyimides/thioimides | 324 | 55.759 | 69.397 | 0.497 |
| Polyamides/thioamides | 401 | 63.238 | 79.479 | 0.273 |
| Polysiloxanes/silanes | 239 | 79.191 | 91.498 | −1.040 |

### Deterioration Across Four Models

For each model and family, the deterioration ratio is:

**MAE deterioration ratio = Family-holdout MAE ÷ Objective-1 MAE (all families)**

The family-level summary averages these four model-specific ratios. It is not a pooled prediction score or the ratio of two model-averaged MAEs.

| Held-out family | Mean MAE deterioration ratio |
|---|---:|
| Polysiloxanes/silanes | 2.995× |
| Polyamides/thioamides | 2.232× |
| Polyimides/thioimides | 2.138× |
| Polysulfides | 2.113× |
| Polyimines | 2.023× |
| Polyvinyls | 1.958× |
| Polyphenylenes | 1.873× |
| Polyurethanes/thiourethanes | 1.817× |
| Polyoxides/ethers/acetals | 1.569× |
| Polycarbonates/thiocarbonates | 1.456× |
| Polyesters/thioesters | 1.447× |

All 11 ratios exceed 1. The comparison demonstrates higher family-holdout errors relative to the overall random-validation reference. Because the two settings contain different test populations and training sets, it does not isolate a causal effect of family exclusion on matched test structures.

## Scientific Insights: Why Does Performance Deteriorate?

### Structural Coverage Is Associated with Transferability

At the individual-prediction level, higher nearest-training similarity is weakly associated with lower absolute error across all four models.

| Model | Predictions | Pearson r | Spearman ρ |
|---|---:|---:|---:|
| Decision Tree | 2,552 | −0.229 | −0.221 |
| Random Forest | 2,552 | −0.245 | −0.230 |
| Extra Trees | 2,552 | −0.236 | −0.214 |
| HistGradientBoosting | 2,552 | −0.225 | −0.196 |

These weak associations show considerable unexplained variation. Similarity is informative about structural coverage, but it does not determine an individual polymer's prediction error.

At the family level, mean nearest-training similarity has the strongest observed association with mean MAE deterioration among the examined factors: **Pearson r = −0.640** and **Spearman ρ = −0.782**.

### Target-Distribution Shifts Also Matter

Absolute differences between training and test median T<sub>g</sub> are positively associated with family-level MAE deterioration: **Pearson r = 0.516** and **Spearman ρ = 0.419**.

Polysiloxanes/silanes combine low mean nearest-training similarity (**0.363**) with a test median **143 °C below** the training median and the largest model-averaged MAE deterioration (**2.995×**).

Polyimides/thioimides also combine low similarity (**0.353**) with a large positive median shift (**157.45 °C**). These observations are consistent with difficulty transferring across structural and property domains.

### A Large Fall in R² Does Not Always Mean the Largest Absolute Error

Polyurethanes/thiourethanes have the largest model-averaged decline in R² (**mean ΔR² = −2.957**) but a smaller MAE deterioration ratio (**1.817×**) than Polysiloxanes/silanes.

Their test/training target IQR ratio is **0.223**, indicating a much narrower central target distribution. Since R² uses test-set variance as its reference, sizeable errors within a narrow target distribution can produce very negative values.

### Model Choice Alone Does Not Resolve the Generalisation Gap

The loss of performance appears across several regression architectures. Changing the algorithm does not automatically supply the missing examples of held-out chemistry.

The findings support reduced structural coverage and target-distribution shift as plausible contributors. They do not establish which factor causes the deterioration or rule out effects from training-set composition, family-specific chemistry and unrecorded material information.

## Practical Recommendations

1. **Match validation to the intended materials application.** Use family or other chemically meaningful holdouts when the intended use involves unfamiliar chemistry.
2. **Report structural coverage alongside predictions.** Nearest-training similarity can provide useful context, but this analysis does not establish a universal acceptance threshold or calibrated uncertainty estimate.
3. **Preserve provenance and source disagreement.** Retain source identifiers, aggregation rules and reported-value ranges so that apparent inconsistencies remain investigable.
4. **Move data-dependent preprocessing inside each training partition.** Repeat validation after fitting descriptor-filtering rules on training data only.
5. **Strengthen comparison design.** Use repeated random splits, family-specific random references and, where feasible, matched test structures to distinguish population effects from exclusion effects.
6. **Improve polymer and experimental metadata.** Seek molecular-weight, composition, tacticity, morphology and measurement information where available.
7. **Evaluate uncertainty and external transfer.** Future work should assess confidence intervals, additional datasets and calibration before using predictions in a screening workflow.

## Key Data Science and Materials-Informatics Concepts Applied

- Structural identity and canonical SMILES.
- Polymer connection markers and multi-label family handling.
- Traceable data aggregation and source-disagreement auditing.
- RDKit molecular descriptors and numerical-validity checks.
- Morgan fingerprints and Tanimoto similarity.
- Supervised regression and ensemble learning.
- Structure-aware splitting and family-level exclusion.
- MAE, RMSE and R² interpretation.
- Interpolation, chemical-domain transfer and applicability limits.
- Pearson and Spearman correlation.
- Target-distribution shift and evidence-based scientific interpretation.

## Relevance to Materials Data Curation and Workflow Engineering

### Joining Materials Experience with Analytics

This project connects my earlier composites and materials-characterisation background with Python-based analysis. It illustrates how experimental context informs structural auditing, interpretation of conflicting reported values and recognition of information absent from a repeat-unit representation.

### Data Quality and Traceability

The workflow documents source records, structural identity, aggregation decisions, multi-label overlap and numerical feature checks. These are practical foundations for maintaining reliable materials datasets.

### Predictive Modelling and Scientific Judgement

The project compares several models, tests chemical transfer and explains why favourable random-validation metrics can be insufficient. It makes the limitations of the evaluation visible alongside the results.

### Reproducibility and Stakeholder Communication

The notebook organises the work from data integrity through molecular features to validation and scientific interpretation. Fixed settings, saved processed data and explicit decision rules support repeatable workflows and technical review.

These capabilities are relevant to materials data curation, research analytics and workflow engineering, where both domain understanding and reliable Python processing are valuable.

## Value of the Project

The project brings together the following tasks:

- Translate a materials-science question into a computational study.
- Audit molecular records before model development.
- Build traceable structure-level datasets.
- Generate and curate molecular representations.
- Compare regression models using appropriate metrics.
- Implement polymer-family exclusion with multi-label safeguards.
- Investigate performance deterioration using structural and distributional evidence.
- Distinguish measured associations from causal explanations.
- Identify concrete improvements to validation and data workflows.
- Communicate technical findings in a clear scientific narrative.

## Tools and Techniques

| Area | Tools and techniques |
|---|---|
| Computing environment | Python, Conda, Jupyter Notebook |
| Data processing | pandas, NumPy |
| Molecular representation | RDKit, canonical SMILES, molecular descriptors, Morgan fingerprints |
| Visualisation | Matplotlib |
| Machine learning | scikit-learn; Decision Tree, Random Forest, Extra Trees, HistGradientBoosting |
| Validation | Random structure-grouped split, polymer-family holdouts |
| Diagnostics | Tanimoto similarity, MAE, RMSE, R², Pearson and Spearman correlations |
| Documentation | Notebook HTML export, GitHub Markdown |

## Project Files

| File | Purpose / status |
|---|---|
| `README.md` | GitHub project overview, methodology, results and interpretation |
| [`results/`](results/) | Supporting CSV tables for family-holdout performance and explanatory analyses; see Supporting Results and Downloadable Tables below |
| [`TehSongXuan_Polymer_Tg_Project1.html`](TehSongXuan_Polymer_Tg_Project1.html) | HTML notebook export containing code, tables and scientific discussion |
| [`TehSongXuan_Polymer_Tg_Project1.ipynb`](TehSongXuan_Polymer_Tg_Project1.ipynb) | Editable Jupyter notebook with saved outputs |
| `Tg_SMILES_class_pid_polyinfo_median (1).csv` | Source-data filename recorded in the notebook; not bundled with this README |
| `data/processed/Tg_structure_level_processed_v1.csv` | Structure-level data export documented in the notebook; not bundled with this README |

The HTML export can be downloaded and opened in a browser. Running the analysis requires the original `.ipynb` notebook, its input files and a compatible environment; the HTML export itself is not executable. The notebook uses paths such as `../data/raw/` and `../results/`, which assume execution from a notebook subfolder. When running it from the repository root, adjust these paths or recreate the expected folder layout.

Dataset redistribution remains subject to the source's applicable terms. Inclusion in this file inventory does not establish that a dataset is available for public redistribution.

## Project Direction

The project connects earlier composites and materials-characterisation experience with Python-based data analysis and machine learning. It uses polymer-property data and RDKit descriptors to predict glass-transition temperature, then compares random structure-grouped validation with polymer-family holdouts.

The central aim is to investigate where predictive performance deteriorates and explain the observed patterns using structural coverage, property-distribution shifts and the limitations of repeat-unit representations. This places scientific interpretation alongside model scores and develops practical foundations for materials data curation and workflow engineering.

## Supporting Results and Downloadable Tables

Supporting analysis outputs are organised in the [`results/`](results/) folder at the top level of this repository, alongside `README.md` and the project notebook. The files are provided in CSV format and can be viewed in GitHub, opened in Microsoft Excel or loaded into Python for further inspection.

| File | Contents |
|---|---|
| [`family_holdout_results.csv`](results/family_holdout_results.csv) | Prediction performance for each regression model under polymer-family holdout validation. |
| [`family_explanation_table.csv`](results/family_explanation_table.csv) | Family-level summary linking performance deterioration with structural coverage, reported glass-transition-temperature distribution shifts and family size. |
| [`family_factor_correlations.csv`](results/family_factor_correlations.csv) | Correlation analysis examining associations between family-level characteristics and deterioration in prediction performance. |
| [`similarity_error_correlations.csv`](results/similarity_error_correlations.csv) | Pearson and Spearman correlations between nearest-training Morgan-fingerprint Tanimoto similarity and absolute prediction error for each model. |

These tables support the notebook’s comparison of random structure-grouped validation and polymer-family holdout validation, together with its investigation of generalisation to unfamiliar polymer chemistry. Correlations are interpreted as associations rather than evidence of causation.

## Limitations and Responsible Interpretation

- **Dataset provenance:** The working file is a third-party processed dataset; its exact relationship to the published collection is not fully established.
- **Representation:** Canonical repeat-unit identity does not uniquely specify a physical polymer sample or resolve every equivalent polymer representation.
- **Missing material context:** Molecular weight, tacticity, composition, morphology and experimental conditions are not consistently encoded.
- **Aggregation:** Median targets provide reproducible structure-level values but compress variation among source measurements.
- **Preprocessing:** Descriptor filtering used the full dataset before validation splitting.
- **Validation scope:** Objective 1 uses one random split; eligible family holdouts cover exclusively labelled test members and do not establish performance for every polymer class or multi-label combination.
- **Comparability:** Holdouts and the overall random reference use different training and test populations.
- **Exploratory diagnostics:** Family-level correlations involve only 11 families, and confidence intervals or causal effects are not established.
- **Operational scope:** The work is a computational generalisation study. External experimental validation, uncertainty calibration and a deployed prediction service have not been demonstrated.

## Conclusion

The curated dataset supports strong prediction under random structure-grouped validation: Extra Trees achieves an MAE of **25.196 °C**, RMSE of **37.092 °C** and R² of **0.886**.

Performance deteriorates when polymer families are excluded from training. Across 11 families, model-averaged MAE deterioration ratios range from **1.447× to 2.995×** relative to each model's overall random-validation reference. Several holdouts produce negative R² values.

Structural coverage and target-distribution shifts provide plausible, exploratory explanations for this gap, while missing polymer and experimental information limits what the representations can capture.

The principal contribution is a traceable demonstration that **successful prediction within familiar chemical space does not establish reliable generalisation to unfamiliar polymer families**. Materials models need validation that reflects the chemistry they are expected to encounter.

## References

1. Uddin, M. J., & Fan, J. (2024). [Interpretable Machine Learning Framework to Predict the Glass Transition Temperature of Polymers](https://doi.org/10.3390/polym16081049). *Polymers, 16*(8), 1049.
2. [Tg SMILES | PID | PolyInfo Class — dataset page](https://www.kaggle.com/datasets/fridaycode/tg-smiles-pid-polyinfo-class). The provenance qualifications above apply to the local working copy.

## Author

**Teh Song Xuan**  
**GitHub:** [tehsongxuan](https://github.com/tehsongxuan)  
**Portfolio areas:** Materials Informatics, Data Curation, Statistical Analysis, Machine Learning and Research Workflow Engineering
