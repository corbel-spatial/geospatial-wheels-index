# Contributing

Issues and pull requests are welcome!

To set up a development environment first install `git` and [uv](https://docs.astral.sh/uv/getting-started/installation/), then:

```shell
git clone https://github.com/corbel-spatial/geospatial-wheels-index
cd geospatial-wheels-index
uv venv
.venv\Scripts\activate
uv pip install -e . --extra dev -r pyproject.toml
uv sync --extra dev
```

To sync from the source repo:

```shell
python sync.py
```

To lint:

```shell
ruff format
```

To test locally:

```shell
pytest
```
