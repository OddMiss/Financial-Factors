[中文](README.md) | English

# Financial-Factors

A collection of notebooks for financial factor research and computation based on financial statements and market data. The repository uses HS300 constituents as examples and covers factor calculation logic, incremental/full computation workflows, and a script & test framework template.

## Contents

- `财报因子v1.ipynb` ~ `财报因子v4.ipynb`: iterative versions of financial-statement factor calculations with implementation notes.
- `财务因子v0.ipynb`: early exploration of financial factor calculations.
- `脚本因子代码测试框架.ipynb`: template framework for factor scripts and test cases.
- `Name-Table.ipynb`: field dictionary and data definitions.
- `Financial Analysis Framework.png`: conceptual framework diagram.
- Reference papers:  
  `The Journal of Finance - June 1992 - FAMA - The Cross‐Section of Expected Stock Returns.pdf`  
  `Do-investors-overvalue-firms-with-bloated-balance-sheets.pdf`

## Key Features

- **Financial factor computation** from balance sheet, income statement, and cash flow data.
- **Incremental & full calculation** consolidated in `财报因子v4.ipynb`.
- **Data handling details** for cumulative values, announcement dates, missing data, and sorting.
- **Script & test templates** to standardize factor development and validation.

## Requirements

The project is organized as Jupyter Notebooks and depends on common Python analytics libraries plus external data interfaces:

- Python 3.x
- numpy, pandas
- statsmodels, matplotlib, seaborn
- `cylib` and `xtdata` (external interfaces for market and financial data)

> `cylib` and `xtdata` are external data interfaces and must be installed/configured in your local environment.

## Usage

1. Ensure access to market and financial statement data (e.g., via `xtdata`).
2. Open a target notebook (start with `财报因子v4.ipynb`).
3. Set key parameters such as `trade_date` and `start_date` as described in the notebook.
4. Run the notebook to compute or validate factors.

## Notes

- Most notebooks use **HS300** constituents as the sample universe.
- Field definitions can be found in `Name-Table.ipynb` and linked dictionaries.

## References

- Fama, E. F., & French, K. R. (1992). The Cross‑Section of Expected Stock Returns.
- Do Investors Overvalue Firms with Bloated Balance Sheets?

