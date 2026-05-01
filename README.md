# Python-Based Financial Modeling & Automation

Automated financial modeling toolkit for valuation, forecasting, DCF analysis,
scenario simulation, and sensitivity analysis.

The project translates standard corporate finance theory into reusable Python
models that reduce manual spreadsheet work and make assumptions easy to audit.

## Features

- Five-year cash flow projection engine
- Discounted cash flow valuation with terminal value
- Base, downside, and upside scenario simulation
- WACC and terminal growth sensitivity table
- Performance metrics such as revenue CAGR, FCF margin, EV/revenue, and EV/EBITDA
- Dependency-free SVG dashboard with forecast, scenario, and metrics graphs
- CSV input/output workflow for repeatable analysis
- CLI overrides for assumptions without editing the CSV
- CLI entry point for running a full valuation report
- Unit tests for valuation math and scenario behavior

## Quick Start


python3 -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
python -m financial_modeling.cli --assumptions data/assumptions.csv --output outputs/valuation_report.csv --chart-output outputs/valuation_dashboard.svg
