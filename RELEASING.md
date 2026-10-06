# Releasing

Publishing is by hand, from a clean clone at the tag. The version in `pyproject.toml` is stamped by
the generator; nothing here is edited.

One-time setup: a PyPI account with two-factor authentication on. The first upload uses the account;
after it, make an API token scoped to the `marketsdk` project and use that.

```bash
python3 -m venv .venv && . .venv/bin/activate
pip install build twine
python -m build
twine upload dist/*
```

Then check `pip index versions marketsdk`.
