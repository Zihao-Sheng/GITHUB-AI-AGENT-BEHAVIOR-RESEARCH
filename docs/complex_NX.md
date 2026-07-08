# complex_NX

`complex_NX.py` is a custom NetworkX visualization helper used in this project to render dense repository-interaction graphs in 2D and 3D.

## Location

```text
src/complex_NX.py
```

Notebook imports should add the project `src/` directory to the Python path before importing:

```python
import sys
from pathlib import Path

sys.path.append(str(Path("..") / "src"))
from complex_NX import NX_style
```

## Purpose

The helper extends standard NetworkX visualization for larger graphs where default layouts can become difficult to read. It supports:

- 2D interactive graph rendering with PyVis;
- 3D interactive graph rendering with Plotly;
- degree-based node sizing and coloring;
- edge coloring by weight or graph attributes;
- weak-edge filtering to reduce visual clutter;
- optional community-based coloring for 2D layouts;
- standalone HTML export.

## Example

```python
import networkx as nx
from complex_NX import NX_style

G = nx.karate_club_graph()

NX_style(
    G,
    mode="2d",
    physics=False,
    height=800,
    width=1200,
    output_html="graph_output.html",
)
```

## Related Files

- `notebooks/06_network_visualization_exploration.ipynb`
- `notebooks/07_complex_nx_2d_drawing_test.ipynb`
- `reports/html/community_2d.html`
- `reports/html/network_3d_example.html`
