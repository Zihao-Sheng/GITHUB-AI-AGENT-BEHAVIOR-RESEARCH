# Data

This directory contains the processed datasets used by the analysis notebooks.

## Processed Files

| File | Description |
| --- | --- |
| `processed/quality.csv` | Pull request records with engineered quality metrics, repository metadata, and the `Y_quality` score used in quality-factor analysis. |
| `processed/failed.csv` | Closed or unsuccessful pull request records used for failure-pattern analysis. |
| `processed/repo_activity.csv` | Repository-level activity, efficiency, popularity, cluster, and network-analysis features. |

## Usage

The notebooks read these files with paths relative to the `notebooks/` directory, for example:

```python
pd.read_csv("../data/processed/quality.csv")
```

## Data Provenance

These files are cleaned and feature-engineered outputs from the original project workflow. The raw extraction pipeline is not included in this repository, so the processed files are retained to make the analysis reviewable and reproducible at the notebook level.
