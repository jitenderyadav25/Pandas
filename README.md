# 🐼 Pandas Learning Notebooks

A collection of Jupyter notebooks I made while learning **pandas**, from the basics (Series and DataFrames) to practical data work like merging, handling missing values, pivot tables, and extracting new features from messy real-world text.

Each notebook is short and focused on one topic, so it can also be used as a quick revision sheet.

---

## 📚 What's Inside

| # | Notebook | What it covers |
|---|----------|----------------|
| 1 | `series.ipynb` | Creating a Series from a list, NumPy array and dictionary; custom index labels |
| 2 | `DataFrames.ipynb` | Creating DataFrames (from dict and list of lists), selecting columns, adding/removing columns and rows, `loc` vs `iloc`, selecting subsets |
| 3 | `Operations.ipynb` | `shape`, `size`, `columns`, `info()`, `describe()`, column arithmetic, applying custom functions with `apply()` |
| 4 | `Missing_data.ipynb` | Detecting missing values (`isna`, `isna().sum()`, `any`), removing them (`dropna`, `thresh`), filling them (`fillna` with a value, a dict, or column means) |
| 5 | `MergingJoiningconcatination.ipynb` | `pd.merge` (inner, outer, left, right), `pd.concat` (rows and columns), `join` |
| 6 | `Groupbyaggregation.ipynb` | Sales dataset set up for GroupBy and aggregation practice *(in progress)* |
| 7 | `Pivot_Tables.ipynb` | `pd.pivot_table` with different aggregations and multiple values, `pd.crosstab` |
| 8 | `FeatureExtraction.ipynb` | Mini project on real data: pulling episode count, air dates and total months out of a messy text column |

---

## 🎌 Mini Project: Feature Extraction on Anime Data

`FeatureExtraction.ipynb` uses `anime.csv` (top 50 anime with `Rank`, `Title` and `Score`). The `Title` column packs several pieces of information into a single string, for example:

```
Fullmetal Alchemist: BrotherhoodTV (64 eps)Apr 2009 - Jul 2010 ...
```

Using custom functions with `apply()`, I extracted new columns:

- **`episode count`**: the number of episodes, cleaned and converted to `int`
- **`Time Stamp`**: the airing period as text
- **`Months`**: total months the show aired, calculated with `datetime` and `relativedelta`

This notebook shows how to turn messy, unstructured text into clean columns that are ready for analysis.

---

## 🛠️ Tech Stack

- Python 3
- pandas
- NumPy
- Jupyter Notebook / JupyterLab

---

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   cd YOUR-REPO-NAME
   ```
2. Install the requirements
   ```bash
   pip install pandas numpy jupyter python-dateutil
   ```
3. Start Jupyter and open any notebook
   ```bash
   jupyter notebook
   ```

> Keep `anime.csv` in the same folder as `FeatureExtraction.ipynb` so the file loads correctly.

---

## 🗺️ Roadmap

- [ ] Complete the GroupBy and aggregation examples (`groupby`, `agg`, multiple keys)
- [ ] Add string and datetime handling notebooks
- [ ] Add a sorting, filtering and conditional selection notebook
- [ ] Build an end-to-end data analysis project with visualisations (Matplotlib / Seaborn)
- [ ] Move on to machine learning with scikit-learn

---

## 🎯 Purpose

I created this repository to practise and document my pandas learning. Feedback and suggestions are welcome. Feel free to open an issue or reach out.

---

## 👤 Author

**Jitender**


⭐ If you find this useful, consider giving the repo a star!
