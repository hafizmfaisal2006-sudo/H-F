# EDA & Preprocessing — Palmer Penguins

Programming for AI — Assignment 2 (Exploratory Data Analysis using Python)

## Files

| File | Description |
|---|---|
| `EDA_Palmer_Penguins.ipynb` | Executed notebook: all 10 tasks (code, output, explanations) and Section 6 answers |
| `penguins.csv` | Original raw dataset (344 rows, 7 columns) |
| `penguins_cleaned.csv` | Final cleaned and encoded dataset (344 rows, 11 columns) |
| `figures/` | Screenshots of the key visualizations |
| `Conclusion.docx` | One-page conclusion |
| `requirements.txt` | Python dependencies |

## How to run

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook EDA_Palmer_Penguins.ipynb
```

Then choose Kernel > Restart & Run All. The notebook reads `penguins.csv` from the same folder.

## Summary of preprocessing

- Missing values: median per species for numeric columns, mode for `sex`
- Duplicates: 0 found
- Categories: text standardized to Title case
- Outliers: none removed (all genuine)
- New feature: `bill_ratio`
- Encoding: label encoding for `sex`, one-hot encoding for `island`
- Scaling: Min-Max and Standard scaling demonstrated (scalers fit on training data only)

Author: HM-FAISAL
