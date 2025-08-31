# Macro Model — Extended Edition

This repository provides a turn‑key macro analytics pipeline that creates synthetic or real macro data, classifies the macro regime, and generates HTML reports with charts.

## Quick start (synthetic)

Run the demo using synthetic data only (no API keys):

```
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m macro_model.cli --demo
```

## Real data via FRED

1. Obtain a FRED API key and set it as an environment variable: `FRED_API_KEY`.
2. Edit `config/sources.yaml`: set `use_synthetic: false` and `fred.enabled: true`.
3. Run the CLI with:

```
python -m macro_model.cli --out reports
```

## Structure

See code for details.
