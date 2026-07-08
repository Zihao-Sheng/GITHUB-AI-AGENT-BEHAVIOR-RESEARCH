# Project Structure

This repository has been reorganized around the final research workflow rather than the original milestone-submission layout.

## Current Layout

```text
.
|-- data/          # processed datasets used by notebooks
|-- notebooks/     # reproducible cleaning, analysis, and visualization notebooks
|-- src/           # reusable Python code
|-- reports/       # final report, archived milestone reports, rendered HTML outputs
|-- docs/          # project and tool documentation
|-- requirements.txt
`-- README.md
```

## Design Rationale

The active project now follows a standard research-analysis structure:

- `data/processed/` keeps analysis-ready CSV files separate from notebooks and reports.
- `notebooks/` uses numeric prefixes to show the workflow order.
- `src/` contains reusable code that is not tied to a single notebook.
- `reports/` stores human-readable outputs, including the final PDF and rendered HTML notebooks.
- `reports/archive/` preserves earlier milestone reports for traceability without making them the main repository interface.
- `docs/` contains supporting documentation for structure and the custom visualization helper.

## Notebook Order

| Notebook | Role |
| --- | --- |
| `01_data_cleaning_quality_and_failures.ipynb` | Cleans pull request data and creates quality/failure datasets. |
| `02_data_cleaning_repository_activity.ipynb` | Builds repository-level activity, efficiency, popularity, and cluster features. |
| `03_quality_factor_analysis.ipynb` | Analyzes factors associated with high-quality agent-generated pull requests. |
| `04_failure_pattern_analysis.ipynb` | Studies common patterns in failed or closed pull requests. |
| `05_repository_network_analysis.ipynb` | Builds and analyzes repository interaction networks. |
| `06_network_visualization_exploration.ipynb` | Explores custom network visualization workflows. |
| `07_complex_nx_2d_drawing_test.ipynb` | Tests 2D rendering behavior for the custom visualization helper. |

## Archived Materials

Earlier course milestone documents are kept in `reports/archive/`:

- `milestone1_plan.pdf`
- `milestone2_report.pdf`

The final written report is `reports/final_report.pdf`.

## Files Intentionally Removed From the Main Tree

The cleanup removed generated and duplicate artifacts that made the repository look like a course-submission bundle:

- notebook checkpoint folders;
- Python bytecode caches;
- source-code zip duplicates;
- duplicate Milestone 2 code and outputs;
- temporary graph-rendering HTML files.

The Git history still preserves previous versions, but the current tree presents the final project clearly.
