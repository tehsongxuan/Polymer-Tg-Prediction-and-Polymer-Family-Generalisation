# Open Materials Data Pipeline for Hydrogel Bioink Design

A reproducible materials-informatics project for curating hydrogel bioink data, preserving experimental context, and deciding whether open records support reliable analysis or machine learning.

Phase 5 hydrogel rheology and printing-context exploratory analysis is complete for the verified Phase 4 evidence layer. The submitted Jupyter run retained 4,600 rheology measurement points, 39,100 source measurement-cell records and 1,031 image-index metadata records; produced 25 scientific PNG figures and 20 CSV analysis tables; and recorded 86 passed validation checks with 0 critical failures. The output remains strictly descriptive: no physical-sample, formulation or rheology-to-image relationship is confirmed, the `mPas` token remains unresolved, and supervised hydrogel prediction is not claimed. The next work is to review the resulting figures and publication permissions, then consider an optional image-file audit or model-artefact audit.

<details>
<summary>Previous Phase 4 checkpoint — retained for project history</summary>

Phase 4 record-linkage-and-analysis-ready evidence-layer execution is complete for the verified Phase 3 checkpoint. The implemented notebook resolves and verifies 21 controlled inputs, maps browser-suffixed filenames back to canonical roles, preserves 39,100 source measurement-cell records, 4,600 measurement-point records and 1,031 image-index records, exports a conservative linkage layer, retains 25 QC findings and 11 unresolved linkage-review rows, and records 0 critical validation failures. Candidate filename correspondences are preserved separately from confirmed physical-sample relationships; no formulation, replicate, rheology-to-image or model-ready target link is asserted. The next step is Phase 5: exploratory rheology and printing-context analysis using only supported populations and clearly stated comparability limits.

</details>

<details>
<summary>Previous Phase 3 checkpoint — retained for project history</summary>
Phase 3 standardisation-and-quality-checks execution is complete for the verified Phase 2 checkpoint. The implemented notebook resolves and verifies the controlled Phase 1/2 inputs by SHA-256, preserves all 39,100 source measurement cells, 4,600 measurement points and 1,031 image-index records, applies only evidence-supported standardisation, retains the unresolved `mPas` viscosity token without conversion, links quality-control findings back to source coordinates, and exports a reproducible Phase 3 handoff. All 674 recorded Phase 3 validation checks passed in the submitted run. Record linkage, rheology interpretation, formulation comparison and modelling remain later work.
</details>

<details>
<summary>Previous Phase 2 checkpoint — retained for project history</summary>
Phase 2 schema-and-quality-control execution is complete for the pinned Phase 1 source snapshot. The implemented notebook verifies the Phase 1 handoff, defines source-grounded entities and identifiers, maps all observed rheology and image-index fields, instantiates traceable prototype tables, applies structural and value-level quality checks, previews supported strain conversion, and carries unresolved scientific questions forward without inventing physical sample links. Full production standardization, evidence-led record linkage, curve fitting, formulation comparison and modelling remain later work.
</details>

<details>
<summary>Previous Phase 1 checkpoint — retained for project history</summary>
Phase 1 source-audit execution is complete for the rheology archive and image-index CSV. The audit produced file and field inventories, source-integrity checks, metadata profiles and a review log. Physical image inspection, experimental sample linkage, unit standardization and modelling remain outside this checkpoint. Phase 2 schema design is the next step.
</details>

<details>
<summary>Original planning status — retained for project history</summary>
**Status:** Proposed. Source feasibility and data audit come first. No analysis or model results are claimed until the source records have been inspected and the planned checks have been completed.
</details>

## Quick navigation

- [Repository home](https://github.com/tehsongxuan/hydrogel-bioink-data-curation)
- [Project overview](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#project-overview)
- [Current status and next step](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#current-status-and-next-step)

### Phase 0 — Scope and source registry

- [Jupyter notebook — scope and source registry](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/00_scope_and_source_registry.ipynb)
- [HTML export — scope and source registry](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/00_scope_and_source_registry.html)
- [View HTML report in browser — scope and source registry](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/00_scope_and_source_registry.html)
- [Phase 0 workflow and methodology](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-0--define-scope-and-register-sources)
- [Phase 0 publication checkpoint](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#github-publication-phase-0-checkpoint)

### Phase 1 — Zenodo source audit

- [Jupyter notebook — Zenodo source audit](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/01_zenodo_source_audit.ipynb)
- [HTML export — Zenodo source audit](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/01_zenodo_source_audit.html)
- [View HTML report in browser — Zenodo source audit](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/01_zenodo_source_audit.html)
- [Phase 1 workflow and methodology](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-1--audit-the-zenodo-source)
- [Phase 1 audit results and scientific interpretation](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-1-audit-results-and-scientific-interpretation)
- [Phase 1 output inventory](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-1-output-inventory)
- [Phase 1 files and publication procedure](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#github-publication-phase-1-checkpoint)

### Phase 2 — Experimental schema and quality control

- [Jupyter notebook — experimental schema and quality control](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/02_schema_and_quality_control.ipynb)
- [HTML export — experimental schema and quality control](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/02_schema_and_quality_control.html)
- [View HTML report in browser — experimental schema and quality control](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/02_schema_and_quality_control.html)
- [Phase 2 workflow and methodology](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-2--design-the-experimental-schema)
- [Phase 2 implementation status](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-2-implementation-status)
- [Phase 2 verified results and scientific interpretation](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-2-verified-results-and-scientific-interpretation)
- [Phase 2 output inventory](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-2-output-inventory)
- [Phase 2 files and publication procedure](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#github-publication-phase-2-checkpoint)

### Phase 3 — Standardisation and quality checks

- [Jupyter notebook — standardisation and quality checks](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/03_standardisation_and_quality_checks.ipynb)
- [HTML export — standardisation and quality checks](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/03_standardisation_and_quality_checks.html)
- [View HTML report in browser — standardisation and quality checks](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/03_standardisation_and_quality_checks.html)
- [Phase 3 workflow and methodology](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-3--standardize-values-and-run-quality-checks)
- [Phase 3 implementation status](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-3-implementation-status)
- [Phase 3 verified results and scientific interpretation](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-3-verified-results-and-scientific-interpretation)
- [Phase 3 output inventory](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-3-output-inventory)
- [Phase 3 files and publication procedure](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#github-publication-phase-3-checkpoint)

### Phase 4 — Record linkage and analysis-ready evidence layer

- [Jupyter notebook — record linkage and analysis-ready evidence layer](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/04_record_linkage_and_analysis_ready_evidence_layer.ipynb)
- [HTML export — record linkage and analysis-ready evidence layer](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/04_record_linkage_and_analysis_ready_evidence_layer.html)
- [View HTML report in browser — record linkage and analysis-ready evidence layer](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/04_record_linkage_and_analysis_ready_evidence_layer.html)
- [Phase 4 workflow and methodology](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-4--assess-record-linkage)
- [Phase 4 implementation status](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-4-implementation-status)
- [Phase 4 verified results and scientific interpretation](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-4-verified-results-and-scientific-interpretation)
- [Phase 4 output inventory](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-4-output-inventory)
- [Phase 4 files and publication procedure](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#github-publication-phase-4-checkpoint)

### Phase 5 — Hydrogel rheology and printing-context exploratory analysis

- [Jupyter notebook — Phase 5 exploratory analysis](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/05_hydrogel_rheology_and_printing_context_analysis.ipynb)
- [HTML export — Phase 5 exploratory analysis](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/05_hydrogel_rheology_and_printing_context_analysis.html)
- [View HTML report in browser — Phase 5](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/05_hydrogel_rheology_and_printing_context_analysis.html)
- [Standalone gallery — all 25 scientific visualisations](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_figure_gallery.html)
- [Figure folder — 25 PNG exports](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/tree/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures)
- [CSV analysis folder — 20 tables](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/tree/main/data/processed/hydrogel_rheology_and_printing_context_analysis)
- [Phase 5 workflow and methodology](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-5--explore-rheology-and-printing-context)
- [Phase 5 verified results and scientific interpretation](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-5-verified-results-and-scientific-interpretation)
- [Complete Phase 5 output inventory — 52 linked deliverables](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#phase-5-complete-linked-file-inventory)
- [Phase 5 files and publication procedure](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md#github-publication-phase-5-checkpoint)

The notebook and HTML export links above point to the canonical files stored in the repository. GitHub may display an HTML file as source text or offer it for download rather than render it as a webpage. The separate **View HTML report in browser** links use HTML Preview to render the same repository HTML files directly in a browser.

## Project overview

Materials research creates records at several levels: ingredients, formulations, processing steps, physical samples, measurements, printing runs, constructs, and images. Those records may live in different tables, instrument exports, archives, and image folders. They are scientifically useful together only when their meanings, units, and relationships are clear.
This project uses an open hydrogel bioink dataset as its experimental case study and uses three complementary materials-informatics resources to practise computational data ingestion, model evaluation, and schema design. The central question is:
> Can open materials records be organized into a traceable workflow that connects documented bioink formulations and processing conditions with rheological measurements and printed-construct information, while preserving the limits of the source data?
The workflow is deliberately data-first: verify sources; audit files; define the data model; validate and standardize values; examine comparable observations; then decide whether prediction is justified. Machine learning is a possible final step, not an assumption made at the beginning.

## Problem statement

The primary experimental source concerns phenol-modified alginate (ALG-Ph) and hyaluronic-acid (HA-Ph) hydrogel inks used in 3D bioprinting. The Zenodo record describes shear-dependent viscosity, storage modulus (`G′`), loss modulus (`G″`), printing metadata, indexed construct images, and files associated with the source authors’ analyses. The planned version is `v0.0.2`, to be checked again before processing. [Zenodo record](https://zenodo.org/records/19602891) · [Dataset DOI](https://doi.org/10.5281/zenodo.19602891)
A rheology file may contain many points from one experiment. Those points are repeated observations, not separate formulations. An image index may describe an image or construct, not an independent material sample. A formulation label may not uniquely identify a physical sample. A successful software join between two tables does not prove they describe the same experiment.
The project therefore asks what each row and file represents, which material and process it describes, and whether a link is supported by source identifiers or documentation. Unexplained rows, missing information, and unmatched records will be recorded rather than silently removed, filled with zero, or forced into a relationship. Keeping these records traceable preserves evidence for review and prevents the curated dataset from appearing more complete or certain than its source.

## Polymer and hydrogel context

A hydrogel is a water-rich polymer network. A bioink is a formulation intended for bioprinting; it may be hydrogel-based and may contain cells, but the word alone does not prove that a dataset includes cells or measures biological performance. The Zenodo case study describes acellular hydrogel printing, so this project will not infer cell viability or tissue response from its rheology or images.
Polymer behaviour depends on more than polymer identity. Concentration, molecular characteristics, chemical modification, additives, crosslinking, processing history, temperature, and test conditions can matter. The source may not report every factor. The project will preserve this incompleteness rather than inventing chemical descriptors or sample conditions.
Rheology describes flow and deformation. Viscosity measures resistance to flow. If viscosity decreases as shear rate increases, the material exhibits shear-thinning behaviour. This can be relevant to extrusion through a printing nozzle, but shear thinning alone does not prove printability. Recovery after extrusion, crosslinking kinetics, nozzle geometry, speed, pressure, and other processing conditions may also matter.
Hydrogels are viscoelastic: their response can include elastic energy storage and viscous energy dissipation. `G′` describes the elastic contribution and `G″` the viscous contribution under the specified oscillatory test conditions. These values should be interpreted alongside information such as frequency, strain, temperature, and sample history. A difference between formulations cannot be attributed to chemistry alone if test conditions or sample identity are uncertain.
The scientific chain of interest is:
**ingredients and polymer chemistry → formulation → processing or crosslinking → measured rheology → printing conditions → construct or documented outcome**
Each connection must be supported by the source. If an identifier or documented convention does not establish a link, it remains unresolved.

## Resources and their roles

The platforms provide different evidence types. They will share data-management and provenance principles, but they will not be merged into one artificial training dataset.
| Resource | Role in this project | Boundary |
|---|---|---|
| [Zenodo bioink dataset](https://zenodo.org/records/19602891) | Primary experimental case study for rheology, printing metadata, and indexed construct images. | Only source-supported links and outcomes will be used. Shape labels and images are not automatically validated print-quality scores. |
| [Materials Project](https://next-gen.materialsproject.org/) | Practise reproducible API retrieval of selected computational materials records, retaining material IDs, query details, returned fields, and calculation provenance. | Its inorganic computational records are not hydrogel rheology measurements and remain in a separate branch. |
| [Matbench](https://matbench.materialsproject.org/) | Reproduce a defined materials-property benchmark to practise controlled model evaluation. The proposed `matbench_dielectric` task predicts refractive index from inorganic crystal structure. | It is not a polymer or hydrogel benchmark; its scores cannot validate a hydrogel model. |
| [Citrine / GEMD](https://citrineinformatics.github.io/gemd-docs/) | Use materials-process-measurement concepts to guide schema design and represent experimental history. | GEMD is a data model, not a hydrogel dataset. Citrination access will be checked before depending on any data there. |
Materials Project provides a Python API client. API retrieval requires an API key, and a query should specify fields that are actually available and needed. The query, selected fields, and retrieval date form part of the provenance record. [API setup](https://docs.materialsproject.org/downloading-data/using-the-api/getting-started) · [Query guidance](https://docs.materialsproject.org/downloading-data/using-the-api/querying-data)
Matbench provides curated tasks for materials-property machine learning. Reproducing its task protocol is a separate exercise in controlled evaluation; it does not transfer a model’s validity from inorganic crystals to polymer networks. [Matbench documentation](https://docs.materialsproject.org/services/ml-and-ai-applications/matbench) · [Matbench repository](https://github.com/materialsproject/matbench)
GEMD helps represent ingredients, materials, processes, measurements, conditions, and results as a connected material history. This can guide the experimental schema even if no Citrination dataset is used. Dataset availability and terms will be checked before any Citrination records are treated as a project input. [GEMD overview](https://citrineinformatics.github.io/gemd-docs/high-level-overview/) · [Citrine Python data model](https://citrineinformatics.github.io/citrine-python/getting_started/data_model.html)

## Linked workflow

Each phase has an input, checks, output, and exit condition. The output from one phase becomes a controlled input to the next. This prevents later plots or models from depending on undocumented joins or guessed unit conversions.

### Phase 0 — Define scope and register sources

**Question:** What does each source contain, and what conclusions can it support?
Record each source URL or DOI, dataset/API identifier, version, retrieval date, access and reuse terms, source type, citation, and local file details or checksum where practical. Confirm the Zenodo version and files; select a bounded Materials Project query; identify the exact Matbench task and protocol; and distinguish Citrine/GEMD documentation from access to Citrination datasets.
**Data-science concept:** provenance starts at acquisition. A property value is not fully described without its source, unit, experiment or material identifier, and processing history.
**Output and handoff:** a project-scope note and source manifest. This manifest controls what is audited in Phase 1 and records the project’s non-goals. Exit when each source and version has a defined, limited purpose.

### Phase 1 — Audit the Zenodo source

**Question:** What files, fields, units, identifiers, and relationships are actually present?
Inventory archives, filenames, formats, tables, columns, row counts, data types, units, labels, IDs, missing values, duplicates, and image files. Compare image names with the image index and read the source documentation for stated record relationships. Separate facts from assumptions: for example, a `shape` label is not automatically a numerical fidelity score.
Log unexpected or unexplained rows, inconsistent labels or units, missing identifiers, and duplicate-looking records. Preserve the original source and record the evidence reviewed. An unusual value is a reason to inspect context, not automatic evidence for deleting or correcting it.
**Data-science concept:** profiling exposes structural problems before transformations or modelling. **Polymer concept:** concentration, crosslinking, and measurement conditions can change the meaning of a rheology value, so the audit checks whether these are measured, reported, or absent.
**Output and handoff:** file and field inventories plus a quality-control issue log. The observed fields and keys—not assumed ones—define Phase 2. Exit when source structure and uncertainty are documented well enough to design the schema.

#### Phase 1 implementation status — 2 October 2026

The executable audit now reads all 92 Excel workbooks directly from `ALG-Ph_HA-Ph_rheology_data.zip` and profiles `image_index.csv`. Manual ZIP extraction is unnecessary. The planned image-file comparison above is deferred: this checkpoint records expected image filenames but does not verify actual image files. Filename correspondence remains candidate evidence rather than a confirmed physical sample relationship.
The original Phase 1 scope above is retained in full. The following results describe only the work implemented and observed in the submitted notebook and HTML export.

## Phase 1 audit results and scientific interpretation

| Audit item | Observed result | Interpretation |
|---|---|---|
| Source files | Rheology ZIP and image-index CSV | Two defined inputs; optional images and model archives are deferred. |
| Reference checksums | Both local MD5 checksums matched the recorded references | Supports file identity against the reviewed source snapshot. |
| Workbook coverage | 92 workbooks and 92 worksheets | 46 modulus workbooks and 46 viscosity workbooks were audited. |
| Measurement records | 4,600 nonblank data rows | Curve points, not 4,600 independent samples or formulations. |
| Image-index records | 1,031 rows | Metadata records; image existence and visual quality were not tested. |
| Strain headers | 44 modulus sheets use `ɣ in -`; 2 use `ɣ in %` | Fraction and percentage representations require explicit handling before comparison. |
| Review register | 15 findings across 7 issue categories | Review items remain visible; findings are not Python execution failures. |
| Audit exports | 11 CSV tables and 1 JSON run manifest | Evidence for schema design and later validation. |
| Input preservation | Source SHA-256 hashes unchanged during execution | The audit did not modify the original ZIP or CSV. |

### Data-science rationale

**Provenance and integrity.** File checksums, archive member paths, workbook sheets and original column headers preserve the origin of observations. A checksum match establishes byte-level agreement with a reference; it does not validate the experimental method or prove that a proposed scientific interpretation is correct.
**Profiling before transformation.** Column profiles describe missing values, numeric content, distinct values and numerical ranges before conversion, imputation or aggregation. The audit preserves unknown information instead of replacing blank metadata with zero or an assumed outcome. It records potential problems so later decisions can cite explicit evidence.
**Granularity and independence.** The 4,600 rows are measurement points nested within rheology workbooks. Treating each point as an independent material would overstate the available evidence and could produce pseudoreplication. Later model evaluation must keep dependent observations together once the source-supported experimental hierarchy is established.
**Record linkage.** Matching workbook stems can suggest a correspondence between viscosity and modulus exports. A matching string does not establish that measurements were made on the same physical sample, batch or replicate. Similarly, an image-index identifier is not automatically a formulation or sample identifier. These distinctions constrain joins and prevent unsupported many-to-many relationships.
**Reproducibility.** The notebook initializes its imports, configuration and audit objects in execution order. It reports the running package versions, reads the two source files and regenerates named outputs instead of appending duplicate results. The submitted export contains completed outputs for all nine code cells and no Python error traceback. Its execution labels are `4, 6, 8, …, 20`; that export alone does not independently verify a fresh-kernel execution sequence.

### Materials-science context

**Strain representation and oscillatory rheology.** Strain is dimensionless, but fraction and percentage are different numerical representations: a strain fraction of 0.01 corresponds to 1%. Source values and headers are retained during the audit. Any later conversion must record its rule and preserve the original unit representation. Comparing unconverted numerical values could introduce a factor-of-100 error.
**Measurement conditions.** Storage modulus `G′` describes elastic energy storage and loss modulus `G″` describes viscous energy dissipation under the specified oscillatory conditions. Their interpretation depends on strain, frequency, temperature and material history. A modulus file must not be called a frequency sweep merely because it contains a frequency column; varying strain at fixed frequency suggests an amplitude-sweep protocol, subject to documentation review. The linear viscoelastic region must be assessed before treating moduli as independent of deformation amplitude.
**Viscosity and complex viscosity.** Steady-shear viscosity and oscillatory complex viscosity describe different measurement modes. Identical-looking units do not establish interchangeability. The source token `mPas` is retained; conversion to Pa·s requires confirmation that it denotes mPa·s. Any correspondence between steady and oscillatory responses requires scientific justification rather than a column-name match.
**Unusual measurements.** Nonpositive rheology values are flagged for review, not automatically deleted, replaced or transformed for plotting. Possible explanations include the measurement range, signal limits or acquisition context, but this audit does not establish their cause. The eight findings are issue-log entries, not a claim that exactly eight individual measurement points are affected.
**Formulation and printing context.** Polymer identity, concentration, chemical modification, crosslinking and processing conditions can affect flow and network response. Missing formulation or irradiation metadata limit interpretation. Blank completeness or reagent annotations remain unknown; they do not prove successful printing, reagent absence or a biological outcome. This checkpoint does not establish causal chemistry–property relationships or cell viability.

### Review findings carried forward

| Issue category | Finding entries | Follow-up |
|---|---:|---|
| `DATASET_LICENCE_UNRESOLVED` | 1 | Confirm the dataset-specific reuse and redistribution terms. |
| `IMAGE_FILES_NOT_AUDITED` | 1 | Audit physical images in a later, explicitly scoped step. |
| `IMAGE_METADATA_BLANK` | 2 | Preserve missingness and review annotation definitions. |
| `INTENSITY_UNIT_UNRESOLVED` | 1 | Establish the source-defined intensity scale and units. |
| `MIXED_STRAIN_UNITS` | 1 | Define traceable fraction/percentage rules in the schema. |
| `NONPOSITIVE_RHEOLOGY_VALUE` | 8 | Review recorded source locations and measurement context. |
| `PHYSICAL_SAMPLE_LINK_UNRESOLVED` | 1 | Seek explicit identifiers or documented relationships. |

### Phase 1 output inventory

All files below are generated locally in `data/metadata/zenodo_source_audit/`. This inventory describes generated outputs; it does not imply that every output has already been committed to GitHub.
| Generated filename | Purpose |
|---|---|
| `source_manifest.csv` | Source identity, selected filenames, reference checksums and input hashes. |
| `archive_member_inventory.csv` | ZIP member paths, sizes and integrity metadata. |
| `workbook_structure_inventory.csv` | Workbook and worksheet structure and row coverage. |
| `source_header_inventory.csv` | Exact source headers and their occurrence counts. |
| `measurement_column_profile.csv` | Column completeness, numeric content and ranges. |
| `measurement_axis_profile.csv` | Observed strain, frequency, shear-rate and temperature coverage. |
| `image_index_column_profile.csv` | Image-index schema and completeness. |
| `image_index_value_counts.csv` | Frequencies of source metadata values. |
| `candidate_filename_correspondences.csv` | Candidate cross-folder filename relationships. |
| `image_filename_expectations.csv` | Expected image filenames; existence remains untested. |
| `audit_issue_log.csv` | Findings, evidence and proposed review actions. |
| `audit_run_manifest.json` | Run timestamp, software versions, counts and file hashes. |

### Phase 2 — Design the experimental schema

**Question:** What real-world entity does one row represent in each table?
Separate formulation records, physical samples if identified, rheology experiments, rheology measurement points, printing events, constructs, and images. One experiment may produce many rheology points; one run may have several images. These are different levels of observation. A replicate in a filename is not proof of physical sample identity unless the source says so.
Define field names, meanings, types, units, allowed values, missing-value semantics, identifiers, and source mapping. A formulation table might hold composition; an experiment table holds test type and conditions; a measurement table holds point-level values. A printing event and image index should be separate if the source supports them. The schema must not invent fields just because they would be useful for modelling.
GEMD concepts can be used as a reference: ingredients enter processes; processes produce or modify materials; measurements characterize materials under conditions and yield results. Intended specifications should be distinguished from what actually occurred in an experimental run.
**Data-science concept:** schema design makes data granularity and relationships explicit. **Polymer concept:** separating material identity, formulation, process, and measurement context keeps the property attached to the conditions that produced it.
**Output and handoff:** schema map, data dictionary, identifier rules, and source-to-schema mapping. These become validation rules for Phase 3. Exit when every field has a definition and each relationship is supported or marked unresolved.

#### Phase 2 implementation status

The original Phase 2 scope above is retained in full. The executed `02_schema_and_quality_control.ipynb` implements a source-preserving schema-validation prototype using the verified Phase 1 checkpoint and the supplied literature context. It does not replace the Phase 1 audit and does not claim that worksheet, filename, image, formulation or printing labels identify independent physical samples.
The implemented scope includes:
- checkpoint integrity verification against the completed Phase 1 manifest;
- an evidence register separating source-reported statements, derived values, interpretation and unresolved questions;
- explicit row granularity and source-coordinate identifier rules;
- source-to-schema mappings for all observed rheology headers and image-index fields;
- four instantiated source-grounded prototype tables;
- explicit missing-value semantics for image metadata;
- a complete executable data dictionary for the prototype fields;
- documented structural, parsing, acquisition-axis, image and unresolved-semantics QC rules;
- value-level QC that retains flagged observations instead of silently cleaning them;
- a traceable strain percent-to-fraction conversion preview;
- a measurement-context and comparability review;
- preservation of all Phase 1 issue records plus Phase 2 decisions and additional review topics; and
- a deterministic export and checksum-based handoff for later standardization and record-linkage work.

This implementation deliberately exercises selected validation concepts described in the conceptual Phase 3 plan because schema rules are more useful when tested against real source records. It does **not** claim that Phase 3 production standardization is complete. Viscosity conversion remains deferred, physical sample linkage remains unresolved, and no rheology-to-image scientific foreign key is created.

## Phase 2 verified results and scientific interpretation

| Phase 2 item | Verified result | Interpretation |
|---|---|---|
| Phase 1 handoff | Two raw files and all eleven Phase 1 audit CSVs matched their recorded SHA-256 values; the reviewed Phase 1 manifest also matched | The Phase 2 schema is tied to the audited source snapshot rather than a silently changed input |
| Reviewed inputs | 19 reviewed inputs registered | Includes data/audit inputs plus supporting publication, supplementary, README, prompt and checkpoint material |
| Source worksheets | 92 | Digital measurement records; not 92 confirmed independent samples |
| Measurement points | 4,600 | Repeated observations within measurement records |
| Source cells | 39,100 | Includes acquisition labels, experimental conditions and measured responses |
| Image-index records | 1,031 | Metadata records; physical image existence was not tested |
| Source-grounded entities | 4 | `worksheet_register`, `measurement_points`, `measurement_values`, and `image_records` |
| Deferred entities | 4 | Formulation, physical sample, printing event and printed construct remain uninstantiated because their identities or relationships are not established |
| Rheology source fields mapped | 13 | Complete mapping of the observed rheology headers |
| Image-index fields mapped | 7 | Complete mapping of the observed image-index schema |
| Core data-dictionary entries | 37 | Every field in the four prototype tables is documented |
| QC rules documented | 14 | Covers checkpoint, source coverage, keys, parsing, response values, acquisition axes, duplicate rows, image metadata, vocabulary, unresolved semantics and strain preview |
| Validation checks | 43 passed | Structural and reconciliation checks passed within the declared contract |
| Value-QC findings | 24 finding records | 20 nonpositive response cells, 2 nonpositive shear-rate cells, and 2 column-level missing-annotation summaries |
| Nonpositive response values | 20 viscosity cells across 8 worksheets | Retained unchanged; their exact source locations reconcile with Phase 1 |
| Nonpositive shear-rate values | 2 cells | Retained as acquisition-axis review flags |
| Image missingness | `completeness_sam`: 943 blanks; `contain_sps`: 922 blanks | Blank remains `unknown_blank`; it is not converted to yes, no, zero, success or reagent absence |
| Strain conversion preview | 2,300 strain cells: 2,200 source-labelled fractions and 100 source-labelled percentages | Percent-to-fraction arithmetic was tested without overwriting source values |
| Modulus acquisition context | All 46 modulus worksheets report fixed 1 Hz frequency with varying strain | Consistent with amplitude-sweep context; no per-curve LVR is assigned |
| Viscosity acquisition context | All 46 viscosity worksheets include a shear-rate value below the publication's nominal lower bound of 0.01 s⁻¹ | Difference is preserved for review rather than removed to match prose |
| Phase 1 findings carried forward | 15 | Original evidence and severity remain visible |
| Additional Phase 2 review topics | 4 | Viscosity unit token, LVR selection, publication-range difference and modelling-population reconciliation remain open |
| Candidate source stems | 62 distinct stems; 30 occur exactly once in each measurement family | Filename correspondence is candidate evidence only |
| Confirmed physical-sample links | 0 | No physical-sample identity or rheology-to-image linkage is asserted |
| Phase 2 exports | 26 CSV files plus 1 JSON run manifest | Reproducible local handoff for later phases |
| Runtime input preservation | All 14 runtime input/checkpoint files remained byte-identical | Phase 2 did not rewrite the raw inputs or Phase 1 checkpoint files |

### Data-science rationale

**Granularity and keys.** The schema distinguishes a source worksheet, a nonblank measurement row, a single source cell and an image-index record. Primary and foreign keys therefore identify digital source coordinates, not physical hydrogel specimens. This prevents the 4,600 curve points from being misrepresented as 4,600 independent materials.
**Source-preserving representation.** Measurement values are retained with their archive member, worksheet, Excel row, source column position, exact source header, source unit and parsing status. A numeric interpretation is added without replacing the original source scalar. This keeps transformation lineage auditable.
**Schema drift and field mapping.** The two observed strain header conventions (`ɣ in -` and `ɣ in %`) are mapped explicitly rather than collapsed silently. All thirteen rheology headers and seven image-index fields must be accounted for, so an unexpected source representation cannot disappear from processing unnoticed.
**Missingness semantics.** Blank image-index values are represented as observed unknowns. The schema does not infer why they are blank and does not convert missing annotations into negative or positive experimental outcomes.
**Referential integrity and reconciliation.** Primary-key, parent-child, row-count, source-coverage, dictionary-coverage and source-header checks validate the internal structure of the prototype. Passing these tests establishes consistency with the reviewed snapshot; it does not prove experimental equivalence or independence.
**QC without silent cleaning.** A warning records a source value or semantic question for review; it does not automatically delete, replace or repair the observation. The 20 nonpositive viscosity values and two negative shear-rate values remain in the data with their source coordinates.
**Traceable transformation.** The strain-conversion preview retains the source scalar and unit, the numerical input, the standardised result, target unit and conversion rule. It demonstrates arithmetic traceability without claiming that all rheology values have been fully standardised.

### Polymer, hydrogel and rheology interpretation

**Oscillatory moduli.** Storage modulus `G′` describes elastic energy storage and loss modulus `G″` describes viscous dissipation under the recorded oscillatory conditions. Because the modulus worksheets show fixed 1 Hz frequency with varying strain, the observed axes are consistent with an amplitude-sweep context rather than a frequency sweep. The notebook does not assign a linear viscoelastic region from the column names alone.
**Strain representation.** Strain is dimensionless, but a percentage and a fraction use different numerical scales. The preview applies `strain_fraction = strain_percent / 100` only where the source explicitly labels the value as percent, while retaining the original representation. Source-labelled fraction values are not clipped merely because their range appears unusual.
**Viscosity.** Steady-shear apparent viscosity and oscillatory complex viscosity are kept distinct. The source token `mPas` is retained because the notebook does not yet establish the instrument notation strongly enough to approve production conversion to Pa·s.
**Measurement context.** Recorded temperature, strain, frequency, shear rate and other acquisition coordinates remain attached to their source measurements. A nominal method statement from the publication does not overwrite an observed workbook value.
**Physical identity and record linkage.** Matching filename stems can support a naming correspondence but do not demonstrate that two files describe the same aliquot, batch, physical sample, rheology specimen, printing run or construct. Phase 2 therefore confirms no physical-sample link.
**Model-readiness boundary.** Successful schema validation is not a machine-learning readiness result. Independent experimental units, validated composition relationships, production unit standardization, defensible record linkage and a prediction target are still unresolved.

### Phase 2 output inventory

The Phase 2 notebook writes its local outputs to `data/metadata/schema_and_quality_control/`. The files below document the executed schema and QC contract. Their existence as local exports does not imply that source-derived tables should all be redistributed publicly.
| Generated filename | Rows | Purpose |
|---|---:|---|
| `input_verification.csv` | 13 | Runtime verification of the two raw inputs and eleven Phase 1 audit CSVs |
| `reviewed_inputs.csv` | 19 | Register of the complete set of reviewed data, checkpoint and supporting documents |
| `literature_evidence_register.csv` | 10 | Evidence statements, scopes and permitted schema decisions |
| `entity_schema.csv` | 4 | Source-grounded entities, row granularity, keys and scientific boundaries |
| `deferred_entities.csv` | 4 | Physical or process entities not instantiated because source evidence is insufficient |
| `source_to_schema_mapping.csv` | 13 | Exact rheology-header mapping, logical type, units and conversion policy |
| `image_field_dictionary.csv` | 7 | Image-index field definitions and semantic limits |
| `data_dictionary.csv` | 37 | Complete field dictionary for the four prototype tables |
| `missing_value_rules.csv` | 5 | Explicit handling rules for blanks, source annotations, structural absence and unresolved semantics |
| `worksheet_register.csv` | 92 | One record per audited source worksheet |
| `measurement_points.csv` | 4,600 | One record per nonblank source measurement row |
| `measurement_values_source.csv` | 39,100 | Source-preserving cell-level measurement and condition table |
| `image_records_source.csv` | 1,031 | Source-preserving image-index metadata table |
| `image_missingness.csv` | 7 | Missingness summary for image-index fields |
| `image_observed_categories.csv` | 81 | Snapshot vocabulary and observed category counts |
| `quality_control_rules.csv` | 14 | Executable QC rule definitions, severities and actions |
| `validation_summary.csv` | 43 | Results of structural and reconciliation checks |
| `value_qc_findings.csv` | 24 | Retained value-level and column-level QC findings |
| `strain_conversion_preview.csv` | 2,300 | Traceable fraction/percentage strain conversion preview |
| `measurement_context_summary.csv` | 6 | Observed acquisition-axis coverage and numerical ranges |
| `context_review.csv` | 3 | Comparability and experimental-context review statements |
| `phase1_issue_carry_forward.csv` | 15 | Original Phase 1 findings retained for history and traceability |
| `phase2_issue_decisions.csv` | 15 | Phase 2 decisions linked to the corresponding Phase 1 findings |
| `additional_review_items.csv` | 4 | Newly recorded open questions requiring later review |
| `filename_candidates_unconfirmed.csv` | 62 | Candidate filename correspondences that are not physical-sample links |
| `linkage_summary.csv` | 3 | Counts summarising candidate naming coverage and confirmed physical-link status |
| `schema_qc_run_manifest.json` | — | Run metadata, software versions, input hashes and output checksums |

### Phase 2 handoff

The verified schema and QC contract is the controlled input to the next project stage. The next work should retain the source values, original unit tokens and unresolved-link statuses while implementing only scientifically justified standardization rules. Production viscosity conversion should wait until the source unit notation is established. Any formulation, sample, printing or image linkage should document the proposed key, supporting evidence, cardinality, unmatched records and physical claim being made.
Phase 2 does not remove the unresolved Phase 1 findings. Dataset-specific reuse terms, physical image inspection, image-annotation semantics, intensity calibration and physical sample linkage remain open. The source archive and source-derived local exports should therefore continue to be handled conservatively until redistribution terms are established.

### Phase 3 — Standardize values and run quality checks

**Question:** Can equivalent information be represented consistently without losing the original evidence?
Standardize field names, labels, types, and units only where meaning is clear. Keep original values and units alongside standardized values, units, and conversion rules. Do not convert an ambiguous unit by guessing. Distinguish zero from not measured, not reported, not applicable, unknown, and unavailable.
Validate required fields, ID uniqueness, foreign keys, duplicate records, numeric types, row counts, unit consistency, and scientifically justified ranges. Treat range checks as flags for review, not automatic correction. Keep a decision trail in the issue log.
**Data-science concept:** executable checks make assumptions repeatable and expose violations. Passing checks does not prove that a scientific relationship is true. **Polymer concept:** `G′` in pascals and viscosity in pascal-seconds describe different properties; even equal units do not ensure comparability if frequency or temperature differs.
**Output and handoff:** standardized tables, validation summary, and transformation lineage. Their verified identifiers support Phase 4. Exit when transformations are reproducible and unresolved problems remain visible.

#### Phase 3 implementation status

The original Phase 3 scope above is retained in full. The executed `03_standardisation_and_quality_checks.ipynb` implements a production standardisation-and-quality-control layer on top of the verified Phase 2 checkpoint. It does not rebuild Phases 1 or 2, does not infer physical sample identity, and does not treat successful software joins as proof of experimental relationships.
The implemented scope includes:
- content-addressed discovery and SHA-256 verification of the raw source files, Phase 1 checkpoint, Phase 2 manifest and all 26 Phase 2 exports;
- runtime recording for Python, pandas, NumPy, openpyxl and IPython;
- exact reconciliation of source coordinates against the original rheology ZIP;
- a 13-rule transformation register tied to the observed Phase 2 source-header mapping;
- source-preserving standardisation of supported numerical quantities;
- percent-to-fraction strain conversion only where the source explicitly uses `%`;
- retention of source-labelled fractional strain without clipping or reinterpretation;
- explicit deferral of `mPas` viscosity conversion because the raw unit token remains insufficiently defined;
- conservative image-metadata handling in which blanks remain `unknown_blank`;
- lossless ISO date-format standardisation for all 1,031 valid source dates without assigning an event meaning;
- carry-forward of all 24 Phase 2 QC finding records plus one Phase 3 document-range review finding;
- source-coordinate links between QC findings and affected observations;
- an observation-preserving 4,600-row point view that keeps rheological acquisition conditions attached;
- deterministic export of 13 CSV tables plus one JSON run manifest; and
- a final preservation check confirming that the protected inputs remained byte-identical.

The notebook is designed for the lifecycle **save → close Jupyter → reopen Jupyter → Restart Kernel → Run All → complete from top to bottom**. Browser-added filename suffixes can be tolerated only when the file bytes match the hashes recorded in the controlled manifests. Scientific identity is therefore established by content rather than by a convenient filename alone.

## Phase 3 verified results and scientific interpretation

| Phase 3 item | Verified result | Interpretation |
|---|---|---|
| Controlled input verification | 41 hash-pinned dependencies resolved and recorded | The Phase 3 run is tied to the raw source snapshot plus the complete Phase 1 and Phase 2 checkpoints rather than to similarly named files |
| Runtime environment | Python 3.12.15; pandas 2.2.3; NumPy 1.26.4; openpyxl 3.1.5; IPython 9.17.1 | Matches the scientific Python stack used by the preceding checkpoint |
| Source worksheets | 92 retained | Digital source records; not 92 independent physical samples |
| Measurement points | 4,600 retained | Nested observations within source worksheets |
| Source measurement cells | 39,100 retained | Original Phase 2 cell-level evidence remains available alongside Phase 3 standardisation fields |
| Image-index records | 1,031 retained | Source metadata records; not automatically formulations, physical samples or validated print-quality outcomes |
| Transformation rules | 13 | One explicit rule per observed rheology source header in the verified mapping |
| Strain cells | 2,300 total: 2,200 source-labelled fractions and 100 source-labelled percentages | Explicit percentages are divided by 100; source-labelled fractions are preserved without clipping |
| Viscosity conversion | 4,600 viscosity cells retained with unresolved `mPas` semantics | No unsupported Pa·s conversion is manufactured |
| Image date format | 1,031 dates standardised losslessly to an additional ISO representation | Format is harmonised without inferring whether the date represents printing, imaging or another event |
| Image missingness | `completeness_sam`: 943 blanks; `contain_sps`: 922 blanks | Blank remains unknown rather than being converted to yes, no, zero, success or reagent absence |
| QC finding records | 25 | The original 24 Phase 2 findings remain visible and one Phase 3 document-range review finding is added |
| QC observation links | 2,302 | Provenance associations between findings and affected source coordinates; not 2,302 samples or independent findings |
| Unresolved review items | 4 | Viscosity notation, LVR selection, publication-range difference and modelling-population reconciliation remain open |
| Phase 3 validation checks | 674 passed | The implemented integrity, transformation, preservation and export contracts passed in the submitted run |
| Phase 3 exports | 13 CSV files plus 1 JSON run manifest | Reproducible local handoff to Phase 4 |
| Physical-sample linkage | Unresolved | No physical-sample, replicate, formulation, printing or rheology-to-image identity is asserted |
| Model readiness | Not established | Passing structural and standardisation checks is not evidence that the data support a leakage-safe predictive model |

### Data-science rationale

**Content-addressed provenance.** Phase 3 accepts controlled inputs by their recorded SHA-256 content rather than trusting a filename alone. This allows a browser-suffixed local copy to be recognised only when it is byte-identical to the expected checkpoint and rejects altered similarly named files.
**Source-preserving transformation.** `measurement_values_standardised.csv` retains every original Phase 2 measurement-value column and adds canonical-field, rule, evidence, standardised-value, standardised-unit and transformation-status fields. A standardised representation therefore does not erase the source scalar, source unit or exact source coordinate.
**Validation versus cleaning.** The workflow tests rules without silently repairing the source. A QC finding remains a review signal. Flagged values are not automatically deleted, clipped, imputed, winsorised or replaced.
**Measurement hierarchy and pseudoreplication.** The 39,100 source cells are nested within 4,600 measurement points and 92 source worksheets. They are not 39,100 independent materials. Preserving this hierarchy is necessary before later summaries, record linkage or model validation.
**Missingness semantics.** Blank image annotations remain observed unknowns. Structural absence, a literal source token, a numeric zero and a deferred transformation are represented differently so later analysis does not manufacture labels from missing metadata.
**Idempotence and reproducibility.** The notebook recreates its named Phase 3 outputs from verified upstream inputs and does not append duplicate records on rerun. The run timestamp may change; the scientific content should remain logically stable for the same controlled inputs.

### Polymer, hydrogel and rheology interpretation

**Strain.** Strain is dimensionless but may be represented as a fraction or percentage. A 1% strain corresponds to a fraction of 0.01. Phase 3 divides by 100 only where the source explicitly labels strain as `%`, and a round-trip check verifies the arithmetic. The source-labelled `ɣ in -` values are retained rather than reinterpreted solely because some values appear unusual.
**Storage and loss moduli.** `G′` represents the elastic contribution and `G″` the viscous/dissipative contribution under the recorded oscillatory conditions. Standardising their representation does not establish gelation, an LVR, printability or equivalence across experiments.
**Viscosity quantities.** Apparent steady-shear viscosity and oscillatory complex-viscosity magnitude `|η*|` remain separate observables. The source token `mPas` is retained because the reviewed evidence does not define the raw export notation strongly enough to approve production conversion to Pa·s.
**Acquisition conditions.** Temperature, strain, frequency, shear rate, time, segment time and stress remain attached to their source observations where present. The same hydrogel can exhibit different measured behaviour under different deformation and thermal conditions, so those axes are part of the scientific meaning of the measurement.
**QC findings.** Nonpositive rheological values and source values outside a nominal publication range remain evidence to review, not automatic reasons for deletion. Their numerical sign or range does not identify the physical cause.
**Record-linkage boundary.** Source-coordinate provenance is not physical-sample identity. Similar filenames, matching stems or a successful software join cannot establish that two records describe the same formulation, batch, aliquot, rheology specimen, printing run or image. Those questions remain Phase 4.

### Phase 3 output inventory

The Phase 3 notebook generated the following local outputs in its standardisation-and-quality-checks output folder. The executed portable run used a `phase3_outputs/standardisation_and_quality_checks/` folder beside the resolved Phase 2 checkpoint because a canonical repository root was not detected. When the canonical repository structure is available, the notebook supports `data/processed/standardisation_and_quality_checks/`. This inventory describes reproducible local outputs; it does not imply that all source-derived tables should be redistributed publicly.
| Generated filename | Rows | Purpose |
|---|---:|---|
| `input_verification.csv` | 41 | Canonical logical paths, resolved local filenames, hashes and verification notes for protected dependencies |
| `document_evidence_register.csv` | 3 | Document-level evidence used for Phase 3 scientific decisions |
| `standardisation_decisions.csv` | 7 | Explicit Phase 3 decisions, evidence and resolution status |
| `phase3_issue_decisions.csv` | 15 | Phase 3 dispositions linked to the carried Phase 1/2 issue history |
| `transformation_rules.csv` | 13 | One machine-readable transformation rule per observed rheology source header |
| `measurement_values_standardised.csv` | 39,100 | Source-preserving long table with added canonical fields, transformation lineage and QC provenance |
| `measurement_points_view.csv` | 4,600 | Convenience view with one row per verified source measurement point |
| `image_records_standardised.csv` | 1,031 | Source-preserving image metadata with conservative date-format and QC additions |
| `qc_findings.csv` | 25 | Carried Phase 2 findings plus the Phase 3 document-range review finding |
| `qc_observation_links.csv` | 2,302 | Finding-to-source-coordinate associations; association count is not an independent-sample count |
| `acquisition_context_coverage.csv` | 18 | Coverage summary for recorded measurement conditions and response fields |
| `unresolved_review_items.csv` | 4 | Open review topics carried forward without forced resolution |
| `validation_summary.csv` | 674 | Complete structured ledger of Phase 3 validation checks |
| `standardisation_run_manifest.json` | — | Runtime, input hashes, output row counts, output hashes, transformation/QC summaries and unresolved decisions |

### Phase 3 handoff

The verified Phase 3 outputs form the controlled computational handoff to conceptual Phase 4. In this project, a **handoff** means that the next workflow stage receives documented, validated outputs together with provenance, transformation rules, QC status and unresolved issues. It does not mean that uncertainty has disappeared or that physical relationships have been proven.
The long standardised measurement table remains traceable to the original archive member, worksheet, Excel row, column position, source header, source scalar and source unit. The point view is a convenience representation, not a replacement for the source-preserving long table. The image table preserves original tokens and missingness states. An empty standardised viscosity value means conversion was deliberately deferred; it does not mean that the source measurement is missing.
The next project stage is evidence-led record linkage in `04_record_linkage_and_analysis_ready_evidence_layer.ipynb`. It should use the verified identifiers and provenance produced here to assess which formulation, rheology, printing and image records can genuinely be connected. Curve fitting, formulation comparison and machine learning should not begin merely because the Phase 3 software checks passed.

### Phase 4 — Assess record linkage

**Question:** Can the curated rheology, image metadata, acquisition context and QC evidence be linked into an analysis-ready materials-informatics evidence layer without inventing physical sample relationships?

Phase 4 evaluates the joinability of the project’s curated records. It connects standardised rheology values, measurement-point records, worksheet provenance, image metadata, QC findings, unresolved review items and Phase 2 filename-candidate evidence while preserving the distinction between a computational key and a scientifically confirmed relationship.

For each candidate relationship, the notebook records the join basis, source evidence, match coverage, unresolved cases and scientific boundary. A successful merge is treated as software evidence only. It does not prove that two records describe the same formulation, prepared sample, aliquot, rheology specimen, printing run or image unless the source data explicitly support that interpretation.

**Data-science concept:** this is record linkage, entity-resolution auditing and join validation. The output defines which fields are safe for descriptive analysis, which are candidate-only evidence, and which must remain excluded from modelling-readiness decisions. **Polymer concept:** formulation-to-rheology or rheology-to-image interpretation requires source-supported material and process identity, not only similar filenames or labels.

**Output and handoff:** a conservative linkage layer, measurement-point linkage view, image-metadata linkage view, candidate linkage table, QC linkage summary, analysis-readiness summary, unresolved-linkage register and validation ledger. Only evidence-supported populations move into Phase 5 exploratory analysis. Exit when each retained relationship has a stated evidence basis and each unsupported relationship remains visibly unresolved.

#### Phase 4 implementation status

The original Phase 4 scope above is retained. The submitted notebook and matching HTML report implement the phase as a reproducible checkpoint named `04_record_linkage_and_analysis_ready_evidence_layer.ipynb`.

The implemented scope includes:
- controlled input resolution for canonical and browser-suffixed filenames, including files such as `input_verification(1).csv`, `validation_summary(2).csv`, `filename_candidates_unconfirmed(2).csv`, `worksheet_register(3).csv`, `ALG-Ph_HA-Ph_rheology_data(5).zip` and `image_index(6).csv`;
- verification of the exact Phase 3 checkpoint and Phase 2 evidence files used for linkage;
- raw-source verification for the rheology archive and `image_index.csv` where available;
- stable source-coordinate keys for worksheet, point and source-cell provenance;
- one row per source measurement point in the measurement-point linkage layer;
- source-cell-level linked measurement evidence with transformation, QC and candidate-linkage context;
- image metadata linkage back to the raw image-index identifiers;
- candidate-only rheology filename correspondences, separated from any physical-sample claim;
- propagation of QC findings and unresolved review items into the Phase 4 evidence layer;
- an analysis-readiness summary that states which fields are safe for Phase 5 descriptive analysis and which remain candidate-only or excluded;
- a run manifest, data dictionary, validation ledger and README summary for reproducible handoff.

## Phase 4 verified results and scientific interpretation

| Phase 4 item | Verified result | Interpretation |
|---|---:|---|
| Controlled input roles resolved | 21 | Required raw, Phase 2 and Phase 3 inputs were located, hashed and mapped to canonical roles. Browser suffixes were recorded instead of ignored. |
| Raw rheology workbook coverage | 92 workbook members | The archive coverage matches the worksheet register used for linkage. |
| Raw image-index coverage | 1,031 image records | Image metadata remained source-grounded; image pixels were not audited in Phase 4. |
| Linked measurement evidence layer | 39,100 rows | Source-cell-level evidence was preserved with provenance, transformation status, QC context and candidate linkage information. These rows are not independent material samples. |
| Measurement-point linkage layer | 4,600 rows | The notebook created one row per verified source measurement point, suitable for Phase 5 descriptive summaries at the correct hierarchy. |
| Image metadata linkage layer | 1,031 rows | Standardised image records were matched back to raw image-index identifiers and source metadata. |
| Candidate rheology-image linkage table | 62 rows | Filename-stem correspondences were retained as candidate evidence only; they are not confirmed rheology-image physical-sample links. |
| QC findings retained | 25 | Phase 4 carried forward the quality-control evidence rather than hiding it during linkage. |
| Unresolved linkage-review rows | 11 | Open and deferred linkage issues remain visible for scientific review. |
| Phase 4 validation checks | 26 | The run created an explicit validation ledger for input resolution, row counts, linkage outputs and boundary conditions. |
| Critical validation failures | 0 | The submitted run completed its declared validation checks without critical failures. |
| Confirmed physical sample linkage | Not asserted | Phase 4 does not claim formulation, replicate, physical-sample, printing-run or rheology-to-image identity where the source does not prove it. |
| Model readiness | Not established | The outputs support Phase 5 exploration and later modelling-readiness review, not immediate prediction. |

### Data-science rationale

**Record linkage is not the same as relationship proof.** Phase 4 separates computational joinability from scientific identity. A shared filename stem, compatible source coordinate or successful table merge can support a candidate relationship, but it does not prove that two records refer to the same physical material or experiment.

**Source-coordinate keys protect provenance.** The linkage layer retains archive member paths, worksheet names, row positions, source headers, source values, units, transformation status and QC context. This allows later plots and summaries to be traced back to source evidence rather than to an unexplained derived table.

**Granularity controls interpretation.** The 39,100 linked measurement rows are source-cell observations nested within worksheets and measurement points. The 4,600 measurement-point rows are a more appropriate level for many descriptive checks, but they still should not be treated as independent formulations or replicate experiments unless later evidence supports that grouping.

**Candidate-only tables reduce overclaiming.** Phase 4 keeps filename-candidate evidence available because it may be useful in Phase 5 review. It also labels that evidence as candidate-only so later analysis does not accidentally turn a naming pattern into a confirmed experimental relationship.

**Analysis readiness is narrower than modelling readiness.** A table can be useful for descriptive analysis while remaining unsuitable for supervised learning. Modelling still requires a defined target, independent experimental units, leakage-safe splits, adequate sample counts and predictors available at the intended prediction time.

### Polymer, hydrogel, rheology and image-metadata interpretation

**Rheology hierarchy.** A rheology workbook may contain many curve points from one acquisition. Viscosity, `G′` and `G″` describe material response under specific test conditions, but each point is not a separate bioink formulation. Phase 4 therefore preserves the nested measurement structure before Phase 5 plots or summaries are attempted.

**Formulation and sample identity remain unresolved.** Polymer identity, concentration, modification, crosslinking and processing history influence hydrogel behaviour. Phase 4 does not create a physical sample ID where the source records do not provide one. This protects later interpretation from attributing measurement differences to formulation variables that may not be uniquely linked.

**Image metadata is not image evidence.** The image-index records include metadata such as image identifier, date, ink type or concentration, shape, irradiation intensity and SPS status where reported. Phase 4 checks metadata linkage only. It does not inspect image files, quantify construct geometry, judge print quality or use images as labels.

**QC context remains part of the science.** Missing annotations, unresolved units, publication-range discrepancies and candidate-only relationships are scientifically meaningful limitations. Keeping them in the evidence layer makes the later analysis more honest and easier to review.

### Phase 4 output inventory

| Output file | Rows | Purpose |
|---|---:|---|
| `phase4_input_file_resolution.csv` | 21 | Maps required canonical inputs to the actual uploaded filenames, file hashes, roles and resolution notes. |
| `linked_measurement_evidence_layer.csv` | 39,100 | Long source-cell-level rheology evidence table with provenance, transformation status, QC context and candidate worksheet linkage. |
| `measurement_point_linkage_layer.csv` | 4,600 | One row per source measurement point with worksheet context and candidate linkage status. |
| `image_metadata_linkage_layer.csv` | 1,031 | Image metadata linked back to raw `image_index.csv` identifiers without auditing image pixels. |
| `candidate_rheology_image_linkage.csv` | 62 | Candidate naming correspondences between rheology and image-related records; no confirmed physical link is asserted. |
| `unresolved_linkage_review_items.csv` | 11 | Open or deferred scientific and linkage questions carried into later review. |
| `qc_linkage_summary.csv` | 25 | Quality-control findings propagated into the Phase 4 linkage context. |
| `analysis_readiness_summary.csv` | 8 | Field- and population-level guidance for Phase 5 descriptive analysis and modelling-readiness boundaries. |
| `phase4_validation_summary.csv` | 26 | Validation ledger for input resolution, output row counts, linkage checks and scientific boundary checks. |
| `phase4_data_dictionary.csv` | 138 | Column-level description of the generated Phase 4 outputs. |
| `phase4_readme_summary.md` | — | Short generated handoff summary, including the optional image-audit note. |
| `phase4_run_manifest.json` | — | Runtime metadata, input-resolution records, output paths, row counts, hashes and validation summary. |

### Phase 4 handoff

The verified Phase 4 outputs form the controlled computational handoff to Phase 5. Phase 5 can use the measurement-point and linked-evidence layers to describe rheology distributions, acquisition coverage and candidate formulation or printing context. It should state the population behind each plot and avoid treating source-cell rows as independent materials.

Candidate filename links may be reviewed and visualised as candidate evidence, but they should not be used as confirmed labels, training targets or ground-truth rheology-image relationships. Image metadata can support coverage and grouping checks; it should not be interpreted as image quality or construct geometry until the actual image files are audited.

### Optional bioink-specific Phase 6 and Phase 7 extensions

The Phase 4 outputs also make two later bioink-specific extensions realistic, provided they remain explicitly optional and source-bounded.

| Optional phase | Extension | What it would do | Required source file |
|---|---|---|---|
| Optional Phase 6 | Image-file audit | Count image files, check the expected `resized_IMG_{image_id}.png` filename pattern, match images to `image_index.csv`, inspect dimensions, colour mode and corruption, review label balance, and optionally compute simple exploratory image features such as area, brightness or edge density. | `images.zip` |
| Optional Phase 7 | Authors’ model and generation-workflow audit | Inventory the authors’ trained model artefacts and fitted rheology-parameter files, compare them with the curated evidence layer, and assess whether beta-CVAE generation or model reproduction is feasible without treating authors’ artefacts as new experimental ground truth. | `models.zip` and `csv_data_files_generation.zip` |

For Optional Phase 6, the image audit would be scoped as:

| Phase 6 section | What it does |
|---|---|
| Image archive audit | Count image files, check filename pattern, and match `resized_IMG_{image_id}.png` to `image_index.csv`. |
| Image metadata QC | Check missing labels, duplicate image IDs, shape distribution and ink formulation distribution. |
| Linkage to curated metadata | Connect image records to Phase 4/5 formulation and printing-condition records where the source evidence supports the link. |
| Basic image inspection | Read dimensions, file integrity, colour mode and corrupted-file status. |
| Optional simple CV features | Calculate area, brightness and edge-density style features for exploratory analysis, not deep learning yet. |

For Optional Phase 7, model comparison remains a reproduction and audit exercise, not proof that the curated Phase 4 tables are ready for supervised hydrogel prediction.

### Phase 5 — Explore rheology and printing context

**Question:** What patterns occur in validated, comparable measurements?
Plot shear-dependent viscosity against shear rate and describe whether the observed curve is consistent with shear-thinning over the measured range. Plot `G′` and `G″` against the source’s measured variable when test conditions allow comparison. Keep individual experiments visible and group summaries at the correct level; do not treat curve points as independent samples.
A derived value such as `tan δ = G″/G′` should be calculated only when both moduli are available and compatible. Record the formula, retain source values, and leave the result undefined when the denominator is zero. Do not alter a measurement to make a derived column complete.
Explore image and printing metadata only if source-defined identifiers link them to rheology or formulation. Define what each image label represents. A requested shape, image category, and validated print-quality outcome are not interchangeable. Describe associations rather than causal effects; unrecorded conditions may explain observed differences.
**Data-science concept:** exploratory analysis describes distributions, coverage, variation, and possible relationships before inference. **Polymer concept:** viscosity, `G′`, and `G″` describe different aspects of flow and viscoelasticity; their printing relevance depends on test and process conditions.
**Output and handoff:** reproducible figures, tables, and a written interpretation with comparability limits. These inform model readiness in Phase 12. Exit when each plot states the source population, unit, condition, and experimental unit.

#### Phase 5 implementation status — 10 October 2026

The original Phase 5 scope and handoff statement above are retained. The submitted `05_hydrogel_rheology_and_printing_context_analysis.ipynb` and matching HTML export document a completed descriptive-analysis checkpoint using the verified Phase 4 evidence layer. The notebook ran in the selected Windows `Python (hydrogel-bioink)` environment, producing the named outputs below. These results refer to that executed run; they are not an independent verification of physical-sample identity or a predictive model.

The implemented workflow includes:
- a kernel-specific start-up check for NumPy, pandas, Matplotlib and IPython, with a bounded one-time Matplotlib installation attempt when it is missing; the executed report says Matplotlib was already available in this particular run;
- documented project-root discovery and controlled input resolution for all ten required Phase 4 CSV/JSON files;
- source-provenance, field-presence, record-count and output-validation checks;
- distinction among 39,100 source-cell evidence rows, 4,600 measurement points and 92 source rheology worksheets, so nested observations are not mistaken for independent formulations;
- exploratory steady-shear curves, log-scale eligibility screening and worksheet-level apparent shear-thinning diagnostics;
- storage modulus `G′`, loss modulus `G″` and valid loss-tangent `tan δ = G″/G′` exploration in the recorded oscillatory strain context;
- summaries of candidate material-name tokens extracted from source filenames without turning them into confirmed formulation IDs;
- independent descriptive analysis of the 1,031 image-index metadata records, without assuming a rheology-to-image join;
- explicit QC propagation, missingness summaries, independent-observation checks, plotting exclusions and unresolved-boundary documentation;
- 25 PNG scientific figures, saved to `figures/`, plus an offline HTML figure gallery; only four previews appear inline to reduce Jupyter display load;
- 20 CSV analysis exports, one JSON run manifest and one generated Markdown summary; and
- a persistent execution-progress log for local troubleshooting, which is **not** a public research deliverable.

## Phase 5 verified results and scientific interpretation

| Phase 5 item | Result in submitted executed notebook | Scientific meaning |
|---|---:|---|
| Required Phase 4 inputs | 10 | Controlled tables and manifest read from the preceding verified evidence layer. |
| Source measurement-cell evidence | 39,100 rows | Original source-cell granularity; **not** 39,100 independent samples. |
| Rheology measurement points | 4,600 rows | 2,300 steady-shear points and 2,300 oscillatory points, nested within worksheets. |
| Source rheology worksheets | 92 | Digital worksheet acquisitions; independent physical specimens have not been established. |
| Image-index metadata | 1,031 records | Categorical and date metadata only; source image pixels were not audited. |
| Candidate filename-linkage records | 62 | Candidate naming correspondence; none confirms a physical sample or rheology-to-image relationship. |
| Carried QC finding records | 25 | Review findings are retained; the number is not a sample count. |
| Measurement points with propagated QC flags | 415 | Flagged source points retained for transparency, rather than silently removed. |
| Unresolved linkage-review entries | 11 | Experimental comparability and identity questions remain open. |
| Steady-shear points eligible for positive log–log plot | 2,280 of 2,300 | 20 source points excluded **from that logarithmic visualisation**, not deleted from curated data. |
| Oscillatory points shown in positive moduli log–log plot | 2,300 | Exploratory point coverage, not confirmation of a linear viscoelastic region. |
| Scientific figures | 25 PNG files | All saved to disk; the notebook shows four selected previews to avoid overloading Jupyter. |
| Analysis outputs | 20 CSV files | Generated population summaries, exploratory curve statistics and QC tables. |
| Additional documentation | 1 HTML gallery, 1 JSON manifest, 1 Markdown summary | Browsable figures and reproducible computational handoff. |
| Phase 5 validation checks | 86 passed | Internal code/data contracts passed in the reported run. |
| Critical validation failures | 0 | Does not resolve outstanding sample, unit or printability questions. |
| Supervised model or validated printability target | Not created | Independent sample units and a defensible training target have not been established. |

### Data-science rationale

**Exploratory analysis and observational hierarchy.** Curves are made of repeated points, and multiple curves can arise from related material preparations. Phase 5 therefore reports results at the point and worksheet levels separately. Counts from `measurement_point_linkage_layer.csv` and source-cell evidence do not establish a dataset with thousands of independent formulations. Treating those points as independent training samples would risk pseudoreplication and optimistic model validation.

**Audit before plotting.** Each log-scale rheology figure requires positive, finite inputs. Twenty steady-shear source points do not satisfy the relevant log–log plotting conditions and are recorded as exclusions for that plot. They remain available in the curated source and QC evidence. A plotting mask is not a silent decision to delete data or identify the cause of an unusual measurement.

**Descriptive slopes are screening measures.** Per-worksheet log–log viscosity slopes describe measured trends over the source acquisition range; they are not fitted constitutive-law parameters validated across material batches. The analysis preserves worksheet-to-worksheet variation and does not claim that apparent trends are chemically causal.

**Provenance-aware visualisation.** The figure atlas includes worksheet coverage, field completeness, QC prevalence, evidence hierarchy, candidate linkage status and source-label coverage. Such diagnostics show what is actually available for analysis, rather than merely making attractive plots. The input manifest and hashes document the Phase 4 data consumed in the run.

**Metadata is not ground truth.** Image-index shape names, reported ink-type strings, irradiation-intensity tokens and dates can be tabulated without claiming to have analysed image pixels, printing performance, geometric fidelity, nozzle conditions or a physical sample-to-image link. The source date field is not assigned a fabricated experimental-event meaning.

### Polymer science, hydrogel rheology and printing-context interpretation

**Steady-shear flow.** Apparent viscosity changes with shear rate and may decrease over the recorded range. A decreasing viscosity curve is consistent with shear-thinning in that measurement window. It is relevant to extrusion-based bioink processing, but alone cannot demonstrate a usable extrusion pressure, structural recovery after deposition or printability. The original `mPas` token remains unresolved and has **not** been converted to Pa·s.

**Oscillatory viscoelastic response.** Storage modulus `G′` represents an elastic response, while loss modulus `G″` represents viscous energy dissipation during oscillation. The submitted dataset's oscillatory analysis treats variation against recorded strain, with a recorded 1 Hz frequency for the reviewed modulus worksheets. These observations are not recast as frequency sweeps. `G′ > G″` at a given point suggests elastic predominance under those measured conditions; it does not by itself establish a gel point, yield stress, print fidelity or a validated linear viscoelastic region.

**Loss tangent.** Where compatible positive values exist, `tan δ = G″ / G′` gives a dimensionless relative measure of viscous and elastic response. A larger tan δ indicates a greater dissipative component *relative to elastic storage* at those conditions. It is undefined when the denominator is zero. Comparing tan δ between unlinked worksheets as if they represented replicates of the same formulation would be unsupported.

**Polymer and process variables.** Alginate and hyaluronic-acid formulation labels are useful for organising review, but source filename tokens are not independently validated composition records. Concentration, chemical modification, crosslinking, processing sequence and thermal history may affect the rheology; an observed difference cannot be attributed to one factor when those factors and physical-sample identities are incompletely linked.

**Printing context.** The source image-index categories describe metadata associated with reported constructs. Their distribution is not a print-quality measurement. Without auditing `images.zip`, measurement protocols, sample identity and source-defined print-quality criteria, Phase 5 does not claim printability prediction, causal formulation–printing relationships, printed geometry accuracy or biological outcomes.

### Phase 5 outputs and handoff

The executed notebook writes its local scientific outputs to:

`data/processed/hydrogel_rheology_and_printing_context_analysis/`

Within that folder, `figures/` holds 25 PNG files, `phase5_figure_gallery.html` indexes those PNGs by relative path, 20 CSVs preserve tabular analyses, `phase5_run_manifest.json` stores run provenance and validation context, and `phase5_readme_summary.md` provides a shorter handoff summary. The generated gallery is not a substitute for the full executed notebook report.

The computational and scientific handoff to a later readiness review includes: documented populations, QC eligibility rules, point/worksheet hierarchy, safe interpretation boundaries and pending sample-linkage questions. Optional Phase 6 can audit actual construct images; Optional Phase 7 can examine the source authors’ model artefacts. Neither extension should reinterpret filename candidates as verified specimen IDs or assume that Phase 5 has produced a supervised training set.

### Phase 5 figure categories

| Category | Figure coverage | Interpretation |
|---|---|---|
| Dataset and hierarchy | Measurement family, worksheet counts, observation levels and field-completeness heatmap | Shows where the scientific evidence comes from and which variables are available. |
| Steady-shear behaviour | Log–log viscosity, individual curves, shear stress, exploratory slopes and exclusion/QC counts | Screens flow properties without claiming a validated constitutive model or printability. |
| Oscillatory mechanics | `G′`, `G″`, tan δ, modulus balance, scatterplot and individual worksheet curves | Distinguishes energy storage and dissipation under recorded test conditions. |
| Candidate naming and linkage | Source-label coverage, presence/absence and filename-linkage status | Candidate labels only; no confirmed physical sample or rheology–image links. |
| Printing/image metadata | Shape, ink type, intensity token, cross-tabulation, annotation missingness and date coverage | Describes index fields, not image pixels, print fidelity or validated quality. |
| Quality control | QC prevalence, measurement field completeness and plot-eligibility diagnostics | Keeps exclusions and scientific uncertainty visible and reproducible. |

The **complete filename-by-filename linked inventory of all 52 Phase 5 publication deliverables** is provided in [GitHub publication: Phase 5 checkpoint](#github-publication-phase-5-checkpoint). These links use proposed canonical repository paths; they only resolve publicly after the respective files are committed. Publication of outputs derived from the third-party dataset is conditional on a separate redistribution/licence review.

### Phase 6 — Audit image files as a bioink-specific extension

**Question:** Do the physical image files match the curated `image_index.csv` metadata, and are they suitable for later exploratory image analysis?

This optional phase uses `images.zip`, which contains resized 800 x 800 printed-construct images. It checks whether expected files such as `resized_IMG_{image_id}.png` are present, whether filenames match image-index identifiers, whether files are readable, and whether metadata labels such as shape, ink type, concentration, irradiation intensity and SPS status have usable coverage.

**Data-science concept:** file-level audit and image-metadata validation must precede computer vision. **Bioink concept:** construct images may support morphology or print-context exploration, but they do not automatically provide print-quality labels or rheology outcomes.

**Output and handoff:** image-file inventory, image-index match report, integrity checks, label-distribution summary and optional simple image features. Exit when image files and metadata can be traced without inventing image-to-rheology identity.

### Phase 7 — Audit authors’ models and generation workflow as a bioink-specific extension

**Question:** Can the authors’ trained models, fitted rheology-parameter files and generation workflow be inventoried or compared reproducibly without treating them as new experimental evidence?

This optional phase uses `models.zip`, `csv_data_files_generation.zip` and the authors’ source-code repository as reference artefacts. It can inspect file structure, model metadata, fitted-parameter tables, expected inputs and reproducibility requirements. It can compare authors’ artefacts with the curated evidence layer only where identifiers and source documentation support the comparison.

**Data-science concept:** model reproduction separates trained artefact inventory, input-data compatibility, environment requirements and evaluation claims. **Materials-informatics concept:** generated images or fitted parameters are derived artefacts; they must not replace source experimental records or create unsupported material labels.

**Output and handoff:** model-artefact inventory, generation-workflow feasibility note, fitted-parameter audit and comparison boundary. Exit when the project can state what is reproducible, what is only partially comparable, and what remains outside the curated experimental evidence layer.

### Phase 8 — Ingest a bounded Materials Project extract

**Question:** Can computational materials records be retrieved and traced reproducibly?
Use the official `mp-api` client for a bounded query. Retain material IDs, query parameters, requested fields, retrieval date, and available calculation provenance. Verify actual returned fields rather than assuming every material has every property. Store API credentials outside version control.
**Data-science concept:** a saved query and source ID make API acquisition reproducible and easier to refresh. **Materials concept:** a calculated inorganic property is a different evidence type from an experimental hydrogel measurement; each keeps its method and provenance.
**Output and handoff:** a documented extract and executable query notebook. This is a separate test case for the metadata design in Phase 11, not a feature table for the hydrogel model. Exit when a reviewer can reproduce the query and identify the origin of each returned value.

### Phase 9 — Reproduce a Matbench task

**Question:** Can a materials-property model be evaluated under a defined protocol?
Reproduce the selected `matbench_dielectric` task using the documented data, folds, and metrics. Its target is refractive index from inorganic crystal structure; despite the name, it is not a hydrogel or polymer dielectric task. Start with a transparent baseline and report features, model, evaluation protocol, and error metrics. Do not tune on the benchmark test data and still call the result a faithful reproduction.
**Data-science concept:** baselines, fixed evaluation procedures, metrics, and leakage checks make results comparable. **Materials-informatics concept:** crystal-structure features do not substitute for polymer chemistry or formulation descriptors.
**Output and handoff:** a reproducible benchmark notebook and score interpretation. The evaluation practices inform Phase 12, but benchmark performance is not evidence that the hydrogel data can support prediction. Exit when task identity, target, inputs, protocol, and limitations are explicit.

### Phase 10 — Map the schema to GEMD

**Question:** Can the documented experimental history be represented as materials, ingredients, processes, measurements, and results?
Map source-supported entities to GEMD concepts. An ingredient may enter a formulation process; a process may create or modify a material; a measurement may be performed on that material under specified conditions. Printing and imaging can be separate processes or records if the source documents them.
GEMD distinguishes intended specifications from experimental runs. A planned concentration is not necessarily the concentration of a prepared and measured sample. A more expressive schema cannot fill a missing sample ID or create evidence absent from the dataset.
**Data-science concept:** knowledge representation captures relationships and constraints that would otherwise remain implicit in column names. **Polymer concept:** formulation and process history can be essential to interpreting a hydrogel’s measured behaviour.
**Output and handoff:** source-to-GEMD mapping, a small example representation, and a list of unsupported fields. This informs common metadata in Phase 11. Exit when mappings do not imply unsupported physical relationships.

### Phase 11 — Apply shared provenance rules

**Question:** What metadata must remain attached so records retain their origin and meaning?
Across the separate source-specific tables, retain source platform and ID, version, source type, material system, property name, original value and unit, standardized value and unit if justified, method, conditions, retrieval date, processing history, and QC status. Distinguish source-reported, transformed, derived, calculated, predicted, and benchmark values.
Record code version, environment, API query, and file checksum where practical. A shared provenance layer supports interoperability; it does not make records scientifically equivalent.
**Data-science concept:** lineage supports audit, debugging, reproducibility, and version updates. **Materials-informatics concept:** consistent metadata can support data exchange while preserving differences among polymer experiments, inorganic calculations, and benchmark tasks.
**Output and handoff:** provenance fields and reusable validation logic. These records allow the final readiness review to rely on traceable evidence. Exit when every processed value can be traced to a source and transformation history.

### Phase 12 — Decide whether hydrogel prediction is justified

**Question:** Do the curated experimental records support a meaningful, independent prediction task?
Define the target before training. “Printability” is not a target until an outcome and measurement method are specified. A source-defined completeness label, objectively calculated shape deviation, or measured rheological property might be candidates if available and consistent. A shape category should not be relabelled as quality without evidence.
Count independent formulations, samples, or printing runs—not just measurement points or image files. Group dependent records together during validation. Check whether predictors are available at the intended prediction time: post-print images cannot serve as predictors for a pre-print decision. Look for target-derived features, missingness, class imbalance, and incompatible measurement conditions.
Possible outcomes are: a defined task is supported; only a restricted task is supportable; or the data support curation and exploration but not reliable prediction. The last outcome identifies which identifiers, measurements, or independent experiments a future dataset would need. If modelling is justified, start with a baseline, grouped validation, error analysis, and a stated domain of applicability.
**Data-science concept:** model readiness depends on target definition, sample size, predictors, leakage-safe validation, and coverage. **Polymer concept:** models need formulation, process, and measurement context; they cannot learn unrecorded chemistry or conditions.
**Output:** a model-readiness report and, only if supported, a limited baseline model. Exit with a defensible statement of what the data can and cannot predict.

## Concepts that connect the phases

- **Data granularity:** define whether a row represents a formulation, sample, experiment, point, run, construct, or image. This guides schema design, summaries, joins, and validation splits.
- **Provenance and lineage:** preserve source identifiers, versions, units, query details, and transformations. This begins in Phase 0 and remains attached through every later output.
- **Missingness semantics:** distinguish zero from unknown, not measured, not reported, not applicable, or unavailable. This affects QC and model feature selection.
- **Standardization:** normalize names and units only with documented rules; keep raw source values available for review.
- **Experimental hierarchy:** points from one curve and images from one run are nested records, not necessarily independent materials. This matters for uncertainty and model evaluation.
- **Leakage control:** related records must not be split carelessly between training and testing. The split should reflect the intended future prediction and the true independent unit.
- **Exploration versus causation:** patterns can motivate hypotheses but do not isolate causal effects when formulation, process, and conditions vary together.

## Planned outputs

Subject to feasibility, the repository may contain:
- Versioned source manifest and file inventory
- Field inventory, data dictionary, and schema map
- Quality-control issue log and validation summary
- Standardized tables with source-to-output traceability
- Record-linkage report with match coverage and unresolved links
- Reproducible notebooks for audit, validation, and exploratory analysis
- Figures and summaries based on validated, comparable observations
- A bioink image-file audit using `images.zip`, if Optional Phase 6 is adopted
- An authors’ model and beta-CVAE workflow audit using `models.zip` and `csv_data_files_generation.zip`, if Optional Phase 7 is adopted
- A bounded Materials Project API-ingestion example
- A Matbench reproduction with documented protocol and metrics
- A GEMD mapping and example representation
- A hydrogel model-readiness report and, only if appropriate, a baseline model

Large source archives and API credentials will not be committed by default. The repository will provide source links, retrieval instructions, environment details, and code for reproducing derived outputs, subject to each provider’s terms.

### Proposed repository structure

```text
open-materials-hydrogel-bioink-pipeline/
├── README.md
├── environment.yml
├── .gitignore
├── DATA_SOURCES.md
├── DATA_DICTIONARY.md
├── PROVENANCE.md
├── notebooks/
│   ├── 00_scope_and_source_registry.ipynb
│   ├── 01_zenodo_source_audit.ipynb
│   ├── 02_schema_and_quality_control.ipynb
│   ├── 03_standardisation_and_quality_checks.ipynb
│   ├── 04_record_linkage_and_analysis_ready_evidence_layer.ipynb
│   ├── 05_hydrogel_rheology_and_printing_context_analysis.ipynb
│   ├── 06_image_file_audit_optional.ipynb
│   ├── 07_authors_model_and_generation_workflow_audit_optional.ipynb
│   ├── 08_materials_project_api_ingestion.ipynb
│   ├── 09_matbench_reproduction.ipynb
│   ├── 10_gemd_mapping.ipynb
│   ├── 11_shared_provenance.ipynb
│   └── 12_model_readiness.ipynb
├── src/
│   ├── ingestion/
│   ├── validation/
│   └── analysis/
├── data/
│   └── metadata/
├── reports/
│   ├── figures/
│   └── tables/
└── docs/
    ├── schema_design.md
    ├── quality_control_rules.md
    └── scientific_boundaries.md
```
This structure is provisional. It will be updated to reflect work actually implemented; listing a notebook here does not claim that it already exists.

### Revised notebook numbering after the implemented Phase 4 checkpoint

The original provisional structure above is retained for project history. The implemented Phase 4 notebook now occupies notebook number `04`, so the later notebook numbers should follow the revised sequence below when those phases are created:
```text
notebooks/
├── 00_scope_and_source_registry.ipynb
├── 01_zenodo_source_audit.ipynb
├── 02_schema_and_quality_control.ipynb
├── 03_standardisation_and_quality_checks.ipynb
├── 04_record_linkage_and_analysis_ready_evidence_layer.ipynb
├── 05_hydrogel_rheology_and_printing_context_analysis.ipynb
├── 06_image_file_audit_optional.ipynb
├── 07_authors_model_and_generation_workflow_audit_optional.ipynb
├── 08_materials_project_api_ingestion.ipynb
├── 09_matbench_reproduction.ipynb
├── 10_gemd_mapping.ipynb
├── 11_shared_provenance.ipynb
└── 12_model_readiness.ipynb
```
This numbering aligns the executable notebook sequence with the implemented Phase 4 checkpoint and the optional bioink-specific image/model extensions. The external Materials Project, Matbench and GEMD work remains separate from the curated hydrogel experimental evidence layer.

## Scientific boundaries

- Materials Project records remain computational and separate from hydrogel experimental data.
- Matbench scores demonstrate benchmark practice, not hydrogel-model validity.
- GEMD guides representation but cannot supply missing source evidence.
- No physical sample or experiment link will be invented.
- Missing values will not be replaced by zero without source justification.
- Unit conversions and derived variables will be traceable to original values.
- Repeated rheology points will not be counted as independent formulations.
- Rheology and images alone will not be used to infer cell viability, tissue function, or clinical performance.
- Observational patterns will not be described as causal effects of polymer chemistry or concentration.
- Modelling will proceed only if the target, independent sample size, record linkage, predictors, and evaluation design support it.
- The project does not claim new polymer synthesis, instrument or sensor development, robotics, or biological testing.

These boundaries shape the source audit, schema, joins, plots, and modelling decision from the beginning.

## Success criteria

The workflow should be able to answer, with evidence: Where did each value originate? What does each row represent? Which values are experimental, computational, derived, or benchmark data? What material, formulation, process, and measurement conditions are documented? Which records can be linked, and which relationships remain uncertain? Which transformations and QC decisions were applied? Which observations are independent? What comparisons are scientifically appropriate? Is there a meaningful, leakage-safe prediction target? What does the dataset support, and what remains unknown?
A finding that the source data are not yet ready for hydrogel machine learning can still be a useful result. It identifies the data gaps that future experiments or repositories need to address.

## Current status and next step

**Current checkpoint:** Phase 5 rheology and printing-context exploratory analysis is complete for the verified Phase 4 data. The executed notebook generated 25 scientific figures and 20 CSV analysis tables; preserved the 4,600-point measurement hierarchy and 1,031 image-index records; carried forward 25 QC findings and 11 unresolved linkage-review entries; and recorded 86 passed validation checks with 0 critical failures. The Phase 5 outputs are descriptive only. The existing unresolved `mPas` unit, sample linkage and image-to-rheology identity boundaries remain. The next step is to review public-release permissions and the completed Phase 5 figure atlas, then decide whether to begin Optional Phase 6 image-file auditing or Optional Phase 7 authors’ model/workflow auditing.
<details>
<summary>Previous Phase 4 checkpoint — retained for project history</summary>
**Current checkpoint:** Phase 4 record-linkage-and-analysis-ready evidence-layer execution is complete. The run resolved 21 controlled inputs, preserved 39,100 source measurement-cell records, 4,600 measurement-point records and 1,031 image-index records, created a 62-row candidate rheology-image linkage table, retained 25 QC findings, exported 11 unresolved linkage-review rows and recorded 0 critical validation failures. It does not assert physical-sample, formulation, replicate, printing-run or rheology-to-image links. The next step is Phase 5: exploratory rheology and printing-context analysis using the Phase 4 evidence layer while keeping candidate-only relationships clearly labelled.
</details>

Optional Phase 6 can audit the actual image archive in `images.zip`. Optional Phase 7 can inventory or compare the authors’ model and beta-CVAE generation artefacts using `models.zip` and `csv_data_files_generation.zip`. These remain separate from Phase 5 and should not be used to claim model readiness before a target, independent unit and validation design are justified.
<details>
<summary>Previous Phase 3 checkpoint — retained for project history</summary>
**Current checkpoint:** Phase 3 standardisation-and-quality-checks execution is complete for the verified Phase 2 checkpoint. The implemented notebook resolves and verifies the controlled Phase 1/2 inputs by SHA-256, preserves all 39,100 source measurement cells, 4,600 measurement points and 1,031 image-index records, applies only evidence-supported standardisation, retains the unresolved `mPas` viscosity token without conversion, links quality-control findings back to source coordinates, and exports a reproducible Phase 3 handoff. All 674 recorded Phase 3 validation checks passed in the submitted run. Record linkage, rheology interpretation, formulation comparison and modelling remain later work.
</details>

<details>
<summary>Previous Phase 2 checkpoint — retained for project history</summary>
**Current checkpoint:** Phase 2 schema-and-quality-control execution is complete for the pinned Phase 1 snapshot. The source-coordinate schema covers all 92 worksheets, 4,600 measurement points, 39,100 source cells and 1,031 image-index records; all 43 recorded validation checks passed. All 15 Phase 1 findings remain traceable, four additional review topics are recorded, and no physical-sample link has been asserted. The next step is Phase 3: implement production standardization and validation only where unit meaning and transformation rules are justified, while preserving unresolved viscosity notation, sample identity, image semantics and publication-range differences. Evidence-led record linkage remains the subsequent Phase 4 task. Physical image review and the Materials Project, Matbench and GEMD extensions remain deferred.
</details>

<details>
<summary>Previous Phase 1 checkpoint — retained for project history</summary>
**Current checkpoint:** Phase 1 execution is complete for the rheology ZIP and image-index CSV, with 15 review findings retained. The next step is Phase 2: define the experimental entities, source-to-schema mappings, original and standardized unit fields, missing-value semantics and evidence requirements for record linkage. Schema design can proceed while unresolved matters remain explicitly recorded. Physical image review and the Materials Project, Matbench and GEMD extensions remain deferred.
</details>

<details>
<summary>Original planning statement — retained for project history</summary>
**Planning and source-feasibility review.** Begin with Phase 0: confirm the Zenodo version and reuse conditions, register the sources, then inspect the primary archive. Finalize the schema, joins, analysis, and any prediction task from the records actually found. Materials Project, Matbench, and GEMD remain separate extensions until the primary audit establishes a manageable scope.
</details>

## GitHub publication: Phase 0 checkpoint

The first publishable checkpoint consists of the project documentation, the Jupyter notebook that checks the working environment and expected project files, and an optional HTML rendering of that notebook. Add the files to the repository using the paths below so these links work on GitHub.
- **Jupyter notebook (executable Python):** [`00_scope_and_source_registry.ipynb`](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/00_scope_and_source_registry.ipynb)
- **HTML notebook export:** [`00_scope_and_source_registry.html`](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/00_scope_and_source_registry.html)
- **Browser-rendered HTML report:** [View `00_scope_and_source_registry.html` in browser](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/00_scope_and_source_registry.html)

The notebook is the editable, rerunnable source. The HTML file is the matching read-only export. The repository link preserves the file in its version-controlled location, while the separate browser-view link uses HTML Preview to render the same report directly in a browser.

### Files for the initial GitHub upload

- `README.md` — this project overview and workflow plan.
- [`notebooks/00_scope_and_source_registry.ipynb`](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/00_scope_and_source_registry.ipynb) — the Phase 0 Jupyter notebook.
- [`reports/00_scope_and_source_registry.html`](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/00_scope_and_source_registry.html) — optional HTML export of the notebook; [view the rendered HTML report in browser](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/00_scope_and_source_registry.html).
- `.gitignore` — recommended to keep local datasets, notebook checkpoints, and environment-specific files out of version control.

Do not include the downloaded Zenodo archive or `image_index.csv` in this initial public upload while reuse and redistribution conditions are being checked. Keep those source files in the local project folder. Additional dataset archives are not required for this Phase 0 checkpoint and can be added to the local project later when downloaded and reviewed.

## GitHub publication: Phase 1 checkpoint

### Core publication files

| File | Repository destination | Direct link |
|---|---|---|
| Updated project README | `README.md` at repository root | [Open README](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md) |
| Executable source-audit notebook | `notebooks/01_zenodo_source_audit.ipynb` | [Open notebook](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/01_zenodo_source_audit.ipynb) |
| Matching HTML report | `reports/01_zenodo_source_audit.html` | [Open HTML export](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/01_zenodo_source_audit.html) · [View rendered HTML in browser](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/01_zenodo_source_audit.html) |
The existing `reports/` convention is retained for both Phase 0 and Phase 1 HTML files. Existing Phase 0 files remain in place. Download suffixes such as `(1)` or `(2)` are removed from the published notebook and HTML filenames so navigation links resolve consistently. A separate `.py` file is not required: the `.ipynb` contains the executable Python cells and the explanatory Markdown.
The 12 generated audit files listed above are additional supporting outputs. They can be reproduced locally from the notebook. They are not required for this documentation-and-code checkpoint; publication of source-derived metadata should follow review of its contents and applicable source terms. The raw ZIP, `image_index.csv`, image archives, model archives and installed environment folders remain local for this checkpoint.

### Execution environment

The submitted run reports Python 3.12.15, NumPy 1.26.4, pandas 2.2.3, openpyxl 3.1.5 and IPython 9.17.1. The selected project kernel is `Python (hydrogel-bioink)`. Its setup excludes user-site package injection to avoid the observed NumPy/pandas binary incompatibility. The notebook includes one-time environment setup and restart instructions. No dependency installation occurs during a routine audit run.
The two required source files are stored locally at:
- `data/raw/zenodo_19602891/ALG-Ph_HA-Ph_rheology_data.zip`
- `data/raw/zenodo_19602891/image_index.csv`

### Browser upload procedure

1. Open [the project repository](https://github.com/tehsongxuan/hydrogel-bioink-data-curation) and select the intended branch, normally `main` for this personal project checkpoint.
2. At the repository root, use **Add file → Upload files** to upload the updated file named exactly `README.md`. Review the change and commit it with a descriptive message.
3. Open `notebooks/`, use **Add file → Upload files**, and choose `01_zenodo_source_audit.ipynb`. Wait until the upload finishes, then commit. Uploading inside this folder avoids placing the notebook at repository root.
4. Return to the repository root, open `reports/`, and upload `01_zenodo_source_audit.html` in the same way. If the folder is absent, **Add file → Create new file** at the root can create `reports/.gitkeep`; commit it, open `reports/`, then upload the HTML. A placeholder is optional after a real file exists.
5. Open the README and check the Phase 1 navigation links. The notebook link should open the executable notebook, the HTML export link should open the stored `01_zenodo_source_audit.html` file, and the separate **View HTML report in browser** link should render the report through HTML Preview.
6. Supporting audit exports, when reviewed and selected for publication, belong together in `data/metadata/zenodo_source_audit/`. Preserve their generated filenames. Upload the actual exports from the local notebook run, not substitute tables from another execution environment.
Suggested commit messages: `Update README with Phase 1 source-audit results`, `Add Phase 1 Zenodo source-audit notebook`, and `Add Phase 1 source-audit HTML report`.
Upload reference: [GitHub documentation — adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).

## GitHub publication: Phase 2 checkpoint

### Core publication files

| File | Repository destination | Direct link |
|---|---|---|
| Updated project README | `README.md` at repository root | [Open README](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md) |
| Executable schema-and-QC notebook | `notebooks/02_schema_and_quality_control.ipynb` | [Open notebook](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/02_schema_and_quality_control.ipynb) |
| Matching HTML report | `reports/02_schema_and_quality_control.html` | [Open HTML export](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/02_schema_and_quality_control.html) · [View rendered HTML in browser](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/02_schema_and_quality_control.html) |
The existing `notebooks/` and `reports/` conventions are retained. Existing Phase 0 and Phase 1 files remain in place. Browser-download suffixes such as `(1)` or `(2)` should be removed from the published Phase 2 notebook and HTML filenames so README links resolve consistently. The canonical public filenames are therefore exactly `02_schema_and_quality_control.ipynb` and `02_schema_and_quality_control.html`.
The notebook is the editable, rerunnable source and contains the executable Python cells together with the scientific and data-science explanation. The HTML report is the matching read-only export. A separate `.py` file is not required for this checkpoint.
The 26 generated CSV files and `schema_qc_run_manifest.json` are reproducible local outputs. Some tables contain source-derived measurement or image-index content. The notebook explicitly treats them as local review products while dataset-specific redistribution terms remain unresolved. They should **not** all be committed automatically merely because they were generated successfully.
The raw rheology ZIP, `image_index.csv`, publication PDF, supplementary document, working prompt, image archives, model archives and installed environment folders remain local unless their redistribution is separately justified. Publication of code and documentation does not imply permission to redistribute third-party source data.

### Phase 2 execution environment

The actual executed environment table in the submitted Phase 2 notebook reports Python 3.12.15, NumPy 1.26.4, pandas 2.2.3, openpyxl 3.1.5 and IPython 9.17.1. The notebook metadata identifies the selected kernel as `Python (hydrogel-bioink)`. No network connection or API key is required for the Phase 2 runtime.
The notebook is designed to be run with **Restart Kernel and Run All**. It reads the original source files and Phase 1 checkpoint files, writes declared outputs only within `data/metadata/schema_and_quality_control/`, and verifies source/checkpoint hashes before and after processing.
The two original source files remain stored locally at:
- `data/raw/zenodo_19602891/ALG-Ph_HA-Ph_rheology_data.zip`
- `data/raw/zenodo_19602891/image_index.csv`

The Phase 1 checkpoint inputs remain under:
- `data/metadata/zenodo_source_audit/`

The Phase 2 generated outputs are written locally to:
- `data/metadata/schema_and_quality_control/`

### Browser upload procedure

1. Open [the project repository](https://github.com/tehsongxuan/hydrogel-bioink-data-curation) and select the intended branch, normally `main` for this personal project checkpoint.
2. At the repository root, use **Add file → Upload files** to upload this updated file named exactly `README.md`. Review the change and commit it with a descriptive message.
3. Open `notebooks/`, use **Add file → Upload files**, and upload the Phase 2 notebook using the canonical filename `02_schema_and_quality_control.ipynb`. Do not keep a browser-download suffix such as `(1)` or `(2)` in the GitHub filename.
4. Return to the repository root, open `reports/`, and upload the matching HTML export using the canonical filename `02_schema_and_quality_control.html`.
5. Open the README and test the Phase 2 navigation links. The notebook link should open the executable `.ipynb`, the HTML-export link should open the stored HTML file, and the separate **View HTML report in browser** link should render the same report through HTML Preview.
6. Keep the raw rheology ZIP, `image_index.csv`, publication files, working prompt and source-derived local prototype tables out of the public upload unless their reuse and redistribution terms have been reviewed and support publication.
7. If selected Phase 2 metadata exports are later approved for publication, preserve the generated filenames and place them together under `data/metadata/schema_and_quality_control/`. Upload outputs from the same verified notebook run rather than reconstructing them manually.
8. After upload, verify that Phase 0 and Phase 1 links still resolve and that no earlier repository files were renamed or removed unintentionally.
Suggested commit messages: `Update README with Phase 2 schema and QC results`, `Add Phase 2 schema and quality-control notebook`, and `Add Phase 2 schema and QC HTML report`.
Upload reference: [GitHub documentation — adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).

## GitHub publication: Phase 3 checkpoint

### Core publication files

| File | Repository destination | Direct link |
|---|---|---|
| Updated project README | `README.md` at repository root | [Open README](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md) |
| Executable standardisation-and-QC notebook | `notebooks/03_standardisation_and_quality_checks.ipynb` | [Open notebook](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/03_standardisation_and_quality_checks.ipynb) |
| Matching HTML report | `reports/03_standardisation_and_quality_checks.html` | [Open HTML export](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/03_standardisation_and_quality_checks.html) · [View rendered HTML in browser](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/03_standardisation_and_quality_checks.html) |
For the Phase 3 public checkpoint, these three files are sufficient: the updated `README.md`, the executable `.ipynb`, and the matching HTML report. Existing Phase 0, Phase 1 and Phase 2 files remain in their current repository locations.
Browser-download suffixes such as `(1)` or `(2)` should be removed from the published filenames. The canonical public Phase 3 filenames are exactly `03_standardisation_and_quality_checks.ipynb` and `03_standardisation_and_quality_checks.html`. The notebook is the editable and rerunnable source; the HTML file is the matching read-only report. A separate `.py` file is not required because the notebook already contains the executable Python cells.
The 13 Phase 3 CSV outputs and `standardisation_run_manifest.json` are reproducible local outputs. Several contain source-derived measurement, image-index or provenance content. Because dataset-specific redistribution remains unresolved, they should **not** all be committed automatically merely because the notebook generated them successfully. The raw rheology ZIP, `image_index.csv`, Phase 1/2 source-derived tables, publication PDF, supplementary document, working prompt, image archives, model archives and installed environment folders also remain local unless their redistribution is separately justified.

### Phase 3 execution environment

The executed Phase 3 report records Python 3.12.15, pandas 2.2.3, NumPy 1.26.4, openpyxl 3.1.5 and IPython 9.17.1. No package installation, network connection or API key is required during the scientific Phase 3 run.
The notebook is designed to be run with **Restart Kernel and Run All** and to remain reproducible after Jupyter is closed and reopened. It resolves protected inputs by content hashes recorded in the Phase 1/2 manifests. Browser-added filename suffixes are accepted only when the file bytes match the expected checkpoint.
A separate Phase 3 `requirements.txt` is not required for this checkpoint. If the repository's existing `environment.yml` already represents the project kernel and has not changed, it does not need to be re-uploaded simply for Phase 3. If the environment file is missing from the repository or later changes, update it as a separate reproducibility task.

### Browser upload procedure

1. Open [the project repository](https://github.com/tehsongxuan/hydrogel-bioink-data-curation) and select the intended branch, normally `main`.
2. At the repository root, use **Add file → Upload files** and upload the updated README using the exact repository filename `README.md`. Commit the change.
3. Open `notebooks/` and upload the Phase 3 notebook using the exact filename `03_standardisation_and_quality_checks.ipynb`. Remove any browser suffix such as `(1)` or `(2)` before or during the upload.
4. Open `reports/` and upload the matching report using the exact filename `03_standardisation_and_quality_checks.html`.
5. Open the updated README and test the new Phase 3 quick-navigation links. The notebook link should open the executable notebook, the HTML-export link should open the stored HTML file, and the **View HTML report in browser** link should render that same report through HTML Preview.
6. Keep the 13 Phase 3 CSV outputs and `standardisation_run_manifest.json` local for now unless selected outputs are separately reviewed for publication and source terms permit redistribution.
7. Keep the raw rheology ZIP, `image_index.csv`, publication files, supplementary material, working prompt and other third-party/source-derived files out of the public Phase 3 upload unless their reuse and redistribution terms have been reviewed and support publication.
8. Verify that Phase 0, Phase 1 and Phase 2 links still resolve and that no earlier files were accidentally renamed or removed.
Suggested commit messages: `Update README with Phase 3 standardisation and QC results`, `Add Phase 3 standardisation and quality-control notebook`, and `Add Phase 3 standardisation and QC HTML report`.
Upload reference: [GitHub documentation — adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).

## GitHub publication: Phase 4 checkpoint

### Core publication files

| File | Repository destination | Direct link |
|---|---|---|
| Updated project README | `README.md` at repository root | [Open README](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md) |
| Executable record-linkage notebook | `notebooks/04_record_linkage_and_analysis_ready_evidence_layer.ipynb` | [Open notebook](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/04_record_linkage_and_analysis_ready_evidence_layer.ipynb) |
| Matching HTML report | `reports/04_record_linkage_and_analysis_ready_evidence_layer.html` | [Open HTML export](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/04_record_linkage_and_analysis_ready_evidence_layer.html) · [View rendered HTML in browser](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/04_record_linkage_and_analysis_ready_evidence_layer.html) |

For the Phase 4 public checkpoint, these three files are sufficient: the updated `README.md`, the executable `.ipynb`, and the matching HTML report. Existing Phase 0, Phase 1, Phase 2 and Phase 3 files remain in their current repository locations.

Browser-download suffixes such as `(1)`, `(2)`, `(5)` or `(6)` should be removed from the published filenames. The canonical public Phase 4 filenames are exactly `04_record_linkage_and_analysis_ready_evidence_layer.ipynb` and `04_record_linkage_and_analysis_ready_evidence_layer.html`. The notebook is the editable and rerunnable source; the HTML file is the matching read-only report. A separate `.py` file is not required because the notebook already contains the executable Python cells.

The ten Phase 4 CSV outputs, `phase4_readme_summary.md` and `phase4_run_manifest.json` are reproducible local outputs. Several contain source-derived measurement, image-index or provenance content. Because dataset-specific redistribution remains unresolved, they should **not** all be committed automatically merely because the notebook generated them successfully. The raw rheology ZIP, `image_index.csv`, Phase 1/2/3 source-derived tables, publication files, working prompts, image archives, model archives and installed environment folders remain local unless their redistribution is separately justified.

### Phase 4 execution environment

The executed Phase 4 manifest records Python 3.12.14 and pandas 2.2.3 on Linux. No package installation, network connection or API key is required during the scientific Phase 4 run.

The notebook is designed to be run with **Restart Kernel and Run All** and to remain reproducible after Jupyter is closed and reopened. It resolves canonical input roles even when uploaded filenames contain browser suffixes, records the actual selected filenames and hashes in `phase4_input_file_resolution.csv`, and writes declared outputs only within `data/processed/record_linkage_and_analysis_ready_evidence_layer/`.

The Phase 4 run expects the verified Phase 3 outputs, the Phase 2 linkage evidence files, and the two raw source files to be available locally. Optional archives `images.zip`, `models.zip` and `csv_data_files_generation.zip` are not required for Phase 4.

### Browser upload procedure

1. Open [the project repository](https://github.com/tehsongxuan/hydrogel-bioink-data-curation) and select the intended branch, normally `main`.
2. At the repository root, use **Add file → Upload files** and upload the updated README using the exact repository filename `README.md`. Commit the change.
3. Open `notebooks/` and upload the Phase 4 notebook using the exact filename `04_record_linkage_and_analysis_ready_evidence_layer.ipynb`. Remove any browser suffix before or during the upload.
4. Open `reports/` and upload the matching report using the exact filename `04_record_linkage_and_analysis_ready_evidence_layer.html`.
5. Open the updated README and test the new Phase 4 quick-navigation links. The notebook link should open the executable notebook, the HTML-export link should open the stored HTML file, and the **View HTML report in browser** link should render that same report through HTML Preview.
6. Keep the generated Phase 4 CSV/JSON/Markdown outputs local for now unless selected outputs are separately reviewed for publication and source terms permit redistribution.
7. Keep `images.zip`, `models.zip` and `csv_data_files_generation.zip` local until Optional Phase 6 or Optional Phase 7 is deliberately started.
8. Verify that Phase 0, Phase 1, Phase 2 and Phase 3 links still resolve and that no earlier files were accidentally renamed or removed.

Suggested commit messages: `Update README with Phase 4 record-linkage results`, `Add Phase 4 record-linkage notebook`, and `Add Phase 4 record-linkage HTML report`.

Upload reference: [GitHub documentation — adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).

## GitHub publication: Phase 5 checkpoint

### Publication scope and the 52-file count

The Phase 5 notebook and matching HTML report form the central public research explanation, consistent with the Phase 0–4 convention. The full **52-file Phase 5 deliverable index** below expands this checkpoint with 25 PNG figures, 20 generated CSV tables, an offline HTML figure gallery, a JSON run manifest, the generated Phase 5 Markdown summary, a Python dependency file and this updated repository README.

**The 52 files are a proposed publication inventory, not a statement that all 52 files have been committed.** Links use canonical intended GitHub paths and will not resolve until the matching file has been uploaded to `main`. Files containing derived source measurement or image-index data must be reviewed for dataset redistribution rights and private local paths before being made public. A source-derived output should remain local if permission is unclear, even when a link is documented as a planned destination.

| Deliverable category | Number | Notes |
|---|---:|---|
| Jupyter notebook | 1 | Editable, executable Python plus scientific Markdown explanations. |
| Executed HTML report | 1 | Read-only export of the verified Phase 5 notebook. |
| Scientific figures | 25 | PNGs generated by the notebook in `figures/`. |
| CSV analysis tables | 20 | Curated exploratory, QC, coverage and validation outputs. |
| Figure gallery HTML | 1 | Local HTML index referring to the adjacent `figures/` directory. |
| Run manifest JSON | 1 | Software, input and output provenance for the executed checkpoint. |
| Phase 5 summary Markdown | 1 | Concise local generated scientific handoff. |
| Python dependency file | 1 | Proposed `requirements-phase5.txt` for environment setup. |
| Updated repository README | 1 | This extended Phase 0–5 project document. |
| **Total Phase 5 files and documentation** | **52** | Each filename is counted exactly once. |

### Core publication files

| File | Repository destination | Direct link |
|---|---|---|
| Updated project README | `README.md` | [Open README](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md) |
| Executable Phase 5 notebook | `notebooks/05_hydrogel_rheology_and_printing_context_analysis.ipynb` | [Open notebook](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/05_hydrogel_rheology_and_printing_context_analysis.ipynb) |
| Matching Phase 5 HTML report | `reports/05_hydrogel_rheology_and_printing_context_analysis.html` | [Open HTML export](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/05_hydrogel_rheology_and_printing_context_analysis.html) · [View rendered HTML in browser](https://htmlpreview.github.io/?https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/05_hydrogel_rheology_and_printing_context_analysis.html) |
| Figure gallery containing all 25 images | `data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_figure_gallery.html` | [Open gallery HTML](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_figure_gallery.html) |
| Run manifest | `data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_run_manifest.json` | [Open manifest](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_run_manifest.json) |
| Phase 5 generated handoff summary | `data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_readme_summary.md` | [Open Phase 5 summary](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_readme_summary.md) |
| Python dependency file | `requirements-phase5.txt` | [Open requirements](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/requirements-phase5.txt) |

The executed HTML notebook report and the figure gallery serve different reading needs. The notebook HTML provides code, explanatory Markdown, tables and four selected inline figure previews; the gallery provides all 25 saved figures. The gallery relies on the `figures/` folder retaining its relative location, so it should not be moved to `reports/` without also updating the figure paths. GitHub's file viewer may show the HTML source or offer a download; for reliable integrated display of gallery and PNGs, configure GitHub Pages with a corresponding self-contained directory after publication permission is cleared.

### Phase 5 complete linked file inventory

Every entry below uses a proposed *canonical repository filename* without browser-added suffixes such as `(3)` or `(4)`. The source of the names is the submitted executed Phase 5 notebook. Direct links are provided for each entry **to be used after the file is committed**.

#### Files 1–3 — README, executable notebook and report

| No. | Deliverable | Canonical GitHub path | Direct link |
|---:|---|---|---|
| 1 | Updated repository README | `README.md` | [Open file](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/README.md) |
| 2 | Jupyter notebook | `notebooks/05_hydrogel_rheology_and_printing_context_analysis.ipynb` | [Open file](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/notebooks/05_hydrogel_rheology_and_printing_context_analysis.ipynb) |
| 3 | Executed HTML report | `reports/05_hydrogel_rheology_and_printing_context_analysis.html` | [Open file](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/reports/05_hydrogel_rheology_and_printing_context_analysis.html) |

#### Files 4–28 — 25 scientific figures

These figures are generated in `data/processed/hydrogel_rheology_and_printing_context_analysis/figures/`. They are organised below in figure-generation order, matching the notebook's progress-log sequence.

| No. | Scientific figure | Direct link | What it shows |
|---:|---|---|---|
| 4 | `phase5_measurement_family_counts.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_measurement_family_counts.png) | Number of source measurement points by measurement family; does not count independent samples. |
| 5 | `phase5_viscosity_vs_shear_rate_loglog.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_viscosity_vs_shear_rate_loglog.png) | Log–log steady-shear viscosity versus shear rate, retaining measurement-level grouping. |
| 6 | `phase5_moduli_vs_strain_loglog.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_moduli_vs_strain_loglog.png) | Oscillatory storage and loss moduli plotted against strain using source-supported axes. |
| 7 | `phase5_tan_delta_vs_strain.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_tan_delta_vs_strain.png) | Derived tan δ over recorded strain where compatible positive moduli permit calculation. |
| 8 | `phase5_candidate_source_label_coverage.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_candidate_source_label_coverage.png) | Coverage of filename-derived candidate ALG-Ph/HA-Ph labels; not verified formulations. |
| 9 | `phase5_image_shape_distribution.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_image_shape_distribution.png) | Distribution of image-index shape labels; not a print-quality assessment. |
| 10 | `phase5_image_intensity_distribution.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_image_intensity_distribution.png) | Source intensity-token counts without unverified unit interpretation. |
| 11 | `phase5_worksheet_point_counts.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_worksheet_point_counts.png) | Measurement-point counts per worksheet, illustrating nesting of curve points. |
| 12 | `phase5_measurement_field_completeness_heatmap.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_measurement_field_completeness_heatmap.png) | Completeness of scientific measurement fields by rheology family. |
| 13 | `phase5_viscosity_quality_and_exclusion_counts.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_viscosity_quality_and_exclusion_counts.png) | Log-scale eligibility and documented exclusions for viscosity curves. |
| 14 | `phase5_viscosity_slope_distribution_and_coverage.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_viscosity_slope_distribution_and_coverage.png) | Exploratory log–log slope distribution and fitting coverage by worksheet. |
| 15 | `phase5_viscosity_example_curve_small_multiples.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_viscosity_example_curve_small_multiples.png) | Selected individual steady-shear curves to expose between-worksheet variation. |
| 16 | `phase5_shear_stress_vs_shear_rate.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_shear_stress_vs_shear_rate.png) | Exploratory source-recorded shear stress versus shear rate. |
| 17 | `phase5_storage_vs_loss_modulus_scatter.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_storage_vs_loss_modulus_scatter.png) | G′ versus G″ relationship for recorded oscillatory points, without independence assumptions. |
| 18 | `phase5_modulus_balance_counts.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_modulus_balance_counts.png) | Counts of data points with G′ larger or smaller than G″. |
| 19 | `phase5_tan_delta_worksheet_medians.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_tan_delta_worksheet_medians.png) | Per-worksheet median tan δ to avoid equating each point with an independent sample. |
| 20 | `phase5_oscillatory_example_curve_small_multiples.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_oscillatory_example_curve_small_multiples.png) | Selected oscillatory curves visualised within their measured strain context. |
| 21 | `phase5_qc_flag_rate_by_family.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_qc_flag_rate_by_family.png) | Proportion of source measurement points with propagated QC context by family. |
| 22 | `phase5_filename_linkage_status_counts.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_filename_linkage_status_counts.png) | Candidate filename-linkage status; not validated physical-sample identity. |
| 23 | `phase5_data_hierarchy_counts.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_data_hierarchy_counts.png) | Distinct evidence tiers (source cells, measurement points, worksheets, image metadata). |
| 24 | `phase5_candidate_label_presence_counts.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_candidate_label_presence_counts.png) | Presence/absence of extractable filename-derived material-label tokens. |
| 25 | `phase5_image_ink_type_top15.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_image_ink_type_top15.png) | Most common image-index ink-type strings; metadata only. |
| 26 | `phase5_image_shape_intensity_heatmap.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_image_shape_intensity_heatmap.png) | Image shape labels cross-tabulated with reported irradiation-intensity tokens. |
| 27 | `phase5_image_metadata_missingness_stacked.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_image_metadata_missingness_stacked.png) | Recorded versus blank image-index annotations; blanks are not negative outcomes. |
| 28 | `phase5_image_metadata_date_coverage.png` | [View PNG](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/figures/phase5_image_metadata_date_coverage.png) | Coverage of source date strings; not assumed printing or measurement dates. |

#### Files 29–48 — 20 CSV analysis tables

These CSV exports are generated under `data/processed/hydrogel_rheology_and_printing_context_analysis/`. Numerical summaries are descriptive, source-dependent outputs. They should not be committed publicly before confirming dataset redistribution terms and inspecting for sensitive or unnecessary local-path columns.

| No. | CSV output | Direct link | Evidence and intended use |
|---:|---|---|---|
| 29 | `phase5_analysis_boundary_table.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_analysis_boundary_table.csv) | Allowed and prohibited interpretations for the analysis populations. |
| 30 | `phase5_candidate_formulation_label_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_candidate_formulation_label_summary.csv) | Counts of combinations of candidate ALG-Ph and HA-Ph filename labels. |
| 31 | `phase5_candidate_label_presence.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_candidate_label_presence.csv) | Counts of whether extractable candidate label tokens occur. |
| 32 | `phase5_candidate_source_label_descriptors.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_candidate_source_label_descriptors.csv) | Filename-stem descriptors for manual review; not verified formulations. |
| 33 | `phase5_data_dictionary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_data_dictionary.csv) | Output file definitions and documentation of Phase 5 exports. |
| 34 | `phase5_field_completeness_by_family.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_field_completeness_by_family.csv) | Non-missing measurement-field coverage by rheology family. |
| 35 | `phase5_image_metadata_descriptive_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_image_metadata_descriptive_summary.csv) | Categorical and numeric summaries of image-index metadata. |
| 36 | `phase5_image_metadata_field_missingness.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_image_metadata_field_missingness.csv) | Image metadata completeness and blank-value counts. |
| 37 | `phase5_image_shape_by_intensity_token.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_image_shape_by_intensity_token.csv) | Cross-tabulation of source shape labels and intensity tokens. |
| 38 | `phase5_input_file_resolution.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_input_file_resolution.csv) | Paths, roles and hashes for 10 required Phase 4 inputs. |
| 39 | `phase5_measurement_family_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_measurement_family_summary.csv) | Rheology family counts, worksheet coverage and source-label coverage. |
| 40 | `phase5_moduli_curve_screening_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_moduli_curve_screening_summary.csv) | Exploratory oscillatory G′/G″ and loss-tangent measures by worksheet. |
| 41 | `phase5_observation_level_hierarchy.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_observation_level_hierarchy.csv) | Counts at each evidence level; repeated curve points are not samples. |
| 42 | `phase5_oscillatory_worksheet_statistics.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_oscillatory_worksheet_statistics.csv) | Per-worksheet oscillatory descriptive and balance statistics. |
| 43 | `phase5_qc_and_boundary_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_qc_and_boundary_summary.csv) | Phase 4 QC findings, unresolved issues and scientific constraints. |
| 44 | `phase5_qc_prevalence_by_rheology_family.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_qc_prevalence_by_rheology_family.csv) | Measurement-point QC prevalence by rheology family. |
| 45 | `phase5_validation_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_validation_summary.csv) | Phase 5 input/output validation ledger and critical-failure status. |
| 46 | `phase5_viscosity_curve_screening_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_viscosity_curve_screening_summary.csv) | Per-worksheet exploratory viscosity trends and log–log slope screening. |
| 47 | `phase5_viscosity_quality_screen.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_viscosity_quality_screen.csv) | Eligibility and exclusions for log-scale viscosity analyses. |
| 48 | `phase5_worksheet_level_evidence_summary.csv` | [Open CSV](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_worksheet_level_evidence_summary.csv) | Worksheet-level record counts and grouping structure. |

#### Files 49–52 — gallery, run manifest, Phase 5 summary and dependencies

| No. | Deliverable | Canonical GitHub path | Direct link | Purpose |
|---:|---|---|---|---|
| 49 | Figure gallery HTML | `data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_figure_gallery.html` | [Open file](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_figure_gallery.html) | Browse all 25 figures; keep adjacent `figures/` relative image paths. |
| 50 | Run manifest JSON | `data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_run_manifest.json` | [Open file](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_run_manifest.json) | Execution provenance, input/output paths, hashes, software versions and validation counts. |
| 51 | Phase 5 summary Markdown | `data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_readme_summary.md` | [Open file](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/data/processed/hydrogel_rheology_and_printing_context_analysis/phase5_readme_summary.md) | Generated concise review handoff from the notebook. |
| 52 | Python dependency file | `requirements-phase5.txt` | [Open file](https://github.com/tehsongxuan/hydrogel-bioink-data-curation/blob/main/requirements-phase5.txt) | Separate documented dependencies for the `hydrogel-bioink` kernel. |

### Adopted Phase 5 repository layout

```text
hydrogel-bioink-data-curation/
├── README.md
├── requirements-phase5.txt
├── notebooks/
│   └── 05_hydrogel_rheology_and_printing_context_analysis.ipynb
├── reports/
│   └── 05_hydrogel_rheology_and_printing_context_analysis.html
└── data/
    └── processed/
        ├── record_linkage_and_analysis_ready_evidence_layer/  # Phase 4 inputs; may remain local
        └── hydrogel_rheology_and_printing_context_analysis/
            ├── figures/                        # 25 named PNGs
            ├── phase5_figure_gallery.html
            ├── phase5_readme_summary.md
            ├── phase5_run_manifest.json
            └── phase5_*.csv                    # 20 named CSVs in inventory
```

The existing repository already includes older notebooks and HTML reports. The tree above shows only the Phase 5 additions; do not delete or rename the earlier Phase 0–4 materials. A separate `.py` file is not required because the `.ipynb` contains the executable Python code.

### Phase 5 execution environment and reproducibility

The uploaded Phase 5 executed notebook reports the selected Windows `Python (hydrogel-bioink)` kernel with Python **3.12.15**, pandas **2.2.3**, NumPy **2.5.3** and Matplotlib **3.11.2**. The environment check prints `Matplotlib found: no package installation required` for that successful run. The notebook contains code that attempts a bounded installation into the **selected Jupyter interpreter** only if Matplotlib is absent. Installation may require network access, and its presence in notebook code is not a guarantee that it can overcome local permissions, network restrictions or incompatible packages.

The local Phase 5 run reads these **ten** Phase 4 input files from `data/processed/record_linkage_and_analysis_ready_evidence_layer/`: `linked_measurement_evidence_layer.csv`, `measurement_point_linkage_layer.csv`, `image_metadata_linkage_layer.csv`, `candidate_rheology_image_linkage.csv`, `qc_linkage_summary.csv`, `analysis_readiness_summary.csv`, `unresolved_linkage_review_items.csv`, `phase4_validation_summary.csv`, `phase4_data_dictionary.csv` and `phase4_run_manifest.json`. Readers who wish to rerun the phase must first reproduce or obtain those files within the source's authorised reuse terms.

For a local run:
1. Put the ten required Phase 4 files in `data/processed/record_linkage_and_analysis_ready_evidence_layer/`.
2. Install the packages recorded in `requirements-phase5.txt` into the same interpreter used by the `hydrogel-bioink` kernel; one-time package installation is distinct from normal notebook execution.
3. Open the canonical Phase 5 `.ipynb` in JupyterLab, select `Python (hydrogel-bioink)`, and use **Restart Kernel and Run All**.
4. Confirm `Dependency and Matplotlib rendering check: PASS`, 25 figure-completion messages, the exported analysis tables, 86 passed checks and zero critical failures in the run's validation summary. A different input dataset or updated code may legitimately produce different counts or reveal a new validation problem.
5. Open the generated `phase5_figure_gallery.html` alongside its `figures/` folder. Review warning messages and the source-provenance boundaries before interpreting any graph.

The notebook also generates `phase5_matplotlib_install.log` and `phase5_execution_progress.log` when relevant. These are **local troubleshooting files**, not part of the 52-file publication inventory, and should not be added to GitHub. The executed notebook and HTML export may include absolute Windows paths in saved outputs; these should be removed or generalised before public release, together with the earlier pandas `DtypeWarning` where practical. Do not replace source-reported values or missingness solely to suppress a warning.

### Reuse, privacy and scientific release conditions

The existing Phase 4 README records that dataset-specific redistribution permission was unresolved. This Phase 5 README deliberately maintains that boundary. Producing CSV files and PNG figures does not in itself grant permission to redistribute source-derived measurement tables, image metadata, or reconstructed data from the Zenodo source. Review the dataset record and accompanying licence/terms first; release only the permitted outputs and attribute the source. If release is not permitted or unclear, **retain the 20 CSV tables, source-derived plots and any problematic manifest content locally** and keep publication to authorised code, descriptions, or aggregate figures where permissible.

Check notebook outputs, HTML reports, data dictionaries, manifests and CSV input-resolution tables for unnecessary local Windows usernames, absolute home directories, account information and temporary paths. Avoid committing installation/progress logs, hidden environment directories, `.ipynb_checkpoints`, cached files, private API keys, source archive ZIPs and the original `image_index.csv` without a separate permission check.

### Browser upload procedure

1. Open [the project repository](https://github.com/tehsongxuan/hydrogel-bioink-data-curation) and select the intended branch, normally `main`. Retain all previously published Phase 0–4 files.
2. Save the updated complete README from this document as the UTF-8 file `README.md` and upload it to the repository root. Because the Phase 5 links are planned paths, some links will not work until their corresponding files are committed.
3. Open `notebooks/` and upload your **reviewed and path-sanitised** Phase 5 `.ipynb` with the exact filename `05_hydrogel_rheology_and_printing_context_analysis.ipynb`, removing a browser suffix such as `(3)`.
4. Open `reports/` and upload its matching, reviewed HTML export as `05_hydrogel_rheology_and_printing_context_analysis.html`, removing a suffix such as `(4)`. The report and notebook should represent the **same executed scientific run**.
5. Upload `requirements-phase5.txt` at the repository root to document the Phase 5 scientific Python dependencies.
6. If the public-release review permits, open/create `data/processed/hydrogel_rheology_and_printing_context_analysis/` and upload the 20 named CSV files, `phase5_run_manifest.json`, `phase5_readme_summary.md` and `phase5_figure_gallery.html`. Preserve those exact filenames.
7. If the figure redistribution review permits, upload the **entire** `figures/` subfolder containing all 25 PNG images in that same output folder. Keep it next to `phase5_figure_gallery.html` so its relative links can resolve.
8. Review the updated README's Phase 5 quick navigation and complete 52-file index, verify any published links, open the notebook, and test the HTML export. For the gallery's embedded images, use a proper served page arrangement such as GitHub Pages after confirming its relative asset paths.
9. Do not upload `phase5_matplotlib_install.log`, `phase5_execution_progress.log`, earlier failed notebook copies, raw archives, source-derived unapproved data, or private environment folders. Treat unapproved table/figure links as planned documentation, not published data.
10. Verify that existing links and Phase 0–4 content were not removed by the README update. Record which Phase 5 files were released and which remain local due to permission or privacy boundaries.

Suggested commit messages: `Update README with Phase 5 hydrogel rheology and printing-context results`, `Add Phase 5 exploratory analysis notebook and HTML report`, `Document Phase 5 Python dependencies`, and, if permitted, `Publish reviewed Phase 5 tables and 25 scientific figures`.

Upload reference: [GitHub documentation — adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).

## Sources and technical documentation

### Experimental hydrogel bioink data

- [Zenodo dataset record](https://zenodo.org/records/19602891)
- [Dataset DOI](https://doi.org/10.5281/zenodo.19602891)
- [Associated publication](https://doi.org/10.1080/17452759.2026.2671497)
- [Authors’ source-code repository](https://github.com/KORINZ/generative-ai-bioprinting-framework)

### Materials Project

- [Materials Project home](https://next-gen.materialsproject.org/)
- [Materials Explorer](https://next-gen.materialsproject.org/materials)
- [General documentation](https://docs.materialsproject.org/)
- [API getting started](https://docs.materialsproject.org/downloading-data/using-the-api/getting-started)
- [API query guidance](https://docs.materialsproject.org/downloading-data/using-the-api/querying-data)
- [Python API client documentation](https://materialsproject.github.io/api/)
- [API client source code](https://github.com/materialsproject/api)

### Matbench and matminer

- [Matbench benchmark and leaderboard](https://matbench.materialsproject.org/)
- [Materials Project Matbench documentation](https://docs.materialsproject.org/services/ml-and-ai-applications/matbench)
- [Matbench source repository](https://github.com/materialsproject/matbench)
- [Matbench methodology paper](https://doi.org/10.1038/s41524-020-00406-3)
- [matminer documentation](https://hackingmaterials.lbl.gov/matminer/)
- [matminer dataset summary](https://hackingmaterials.lbl.gov/matminer/dataset_summary.html)

### Citrine, GEMD, and Citrination

- [Citrine Informatics](https://citrine.io/)
- [Citrine DataManager](https://citrine.io/platform/citrine-datamanager/)
- [GEMD documentation](https://citrineinformatics.github.io/gemd-docs/)
- [GEMD high-level overview](https://citrineinformatics.github.io/gemd-docs/high-level-overview/)
- [Citrine Python data-model overview](https://citrineinformatics.github.io/citrine-python/getting_started/data_model.html)
- [gemd-python source repository](https://github.com/CitrineInformatics/gemd-python)
- [Citrination](https://citrination.com/) — included as a platform reference; dataset availability and access will be verified before use.

