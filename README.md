# cf-graph
Repo for holding the conda-forge dependency graph and its introspection.

Note that this repos is mostly bot managed and operated.

Please open issues in [cf-scripts](https://github.com/regro/cf-scripts/issues).

## code snippets to test building the graph

```python
from conda_forge_tick.make_graph import make_graph
from conda_forge_tick.all_feedstocks import get_all_feedstocks
from conda_forge_tick.utils import load_graph

names = get_all_feedstocks(cached=True)[0:10]
gx = load_graph()
make_graph(names, gx)
```
