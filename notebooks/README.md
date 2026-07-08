# Notebooks

The notebooks are ordered to match the research workflow.

| Notebook | Purpose |
| --- | --- |
| `01_data_cleaning_quality_and_failures.ipynb` | Cleans pull request records and constructs quality/failure datasets. |
| `02_data_cleaning_repository_activity.ipynb` | Builds repository-level activity, efficiency, popularity, and cluster features. |
| `03_quality_factor_analysis.ipynb` | Studies factors associated with higher-quality AI-agent-generated pull requests. |
| `04_failure_pattern_analysis.ipynb` | Analyzes common patterns in closed or unsuccessful pull requests. |
| `05_repository_network_analysis.ipynb` | Builds and visualizes repository interaction networks. |
| `06_network_visualization_exploration.ipynb` | Explores custom large-network visualization workflows. |
| `07_complex_nx_2d_drawing_test.ipynb` | Tests 2D rendering behavior for `complex_NX`. |

Run notebooks from this directory. Processed data is read from `../data/processed/`, and reusable code is imported from `../src/`.
