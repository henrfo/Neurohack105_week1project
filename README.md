# Neurohack105 — Week 1 Project

## Setup

Everything is managed by [uv](https://docs.astral.sh/uv/). Clone, then:

```bash
uv sync
```

That creates `.venv/` and installs the exact versions pinned in `uv.lock`. No manual venv activation needed.

## Running things

```bash
uv run jupyter lab          # start JupyterLab
uv run python script.py     # run any script
```

In JupyterLab, pick the kernel named **neurohack105-week1**.

## Adding a package

```bash
uv add seaborn              # updates pyproject.toml + uv.lock and installs
uv remove seaborn
```

Commit `pyproject.toml` and `uv.lock` so the environment stays reproducible.

## Notes

- PyTorch uses the Apple Silicon GPU via the `mps` device.
- `data/` is gitignored — keep raw data out of the repo.
