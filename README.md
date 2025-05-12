# try-point-blank

Try Pointblank - https://posit-dev.github.io/pointblank/

- [try-point-blank](#try-point-blank)
  - [Status](#status)
  - [Overview](#overview)
    - [Key Artefacts](#key-artefacts)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)

## Status

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)

## Overview

This project demonstrates data validation in Python using Posit's `pointblank`, a new open-source library inspired by its popular R counterpart.

Ensuring data quality is essential for trustworthy analytics, decision-making, and data governance. pointblank makes it easy to define validation rules for `Pandas`, `Polars`, and `DuckDB` tables, generating clear, actionable reports.

Compared to other tools like Great Expectations, Pandera, and Deequ, `pointblank` stands out for its intuitive API, seamless integration with modern Python data stacks, and robust reporting features. The package enables you to check for missing values, validate ranges and categories, and extract failing records for further inspection. It also supports advanced features like threshold-based monitoring and custom actions on validation failures.

This repository includes example validations (using the classic Titanic dataset) and demonstrates how to leverage pointblank for practical data quality workflows. See the accompanying code and documentation for details on setup, rule definition, and report generation.

For a complete write up, see this [blog post](https://www.databooth.com.au/posts/pointblank/).

### Key Artefacts

- **[`notebooks/titanic.ipynb`](notebooks/titanic.ipynb)**: The main notebook that demonstrates the functionality of `pointblank` with the Titanic dataset.
- **`notebooks/titanic.duckdb`**: The DuckDB database file containing the Titanic dataset.
- **`LICENSE`**: The Apache License 2.0 under which this project is distributed.

## Getting Started

### Prerequisites

- Python 3.10 or higher
- `pointblank`
- `duckdb`
- `pandas`
- `notebook` (including IPython) for displaying Markdown in notebooks

Install the required dependencies using `uv`:

```bash
uv add pointblank duckdb pandas ipython
```
