# Python for Data Science

Notebooks for a Python programming course in a data-science specialization. Each
week is a self-contained Jupyter notebook mixing explanations with runnable examples.

## Setup

```bash
conda create -n pyds python=3.11
conda activate pyds
pip install numpy pandas matplotlib scipy scikit-learn networkx xgboost seaborn folium jupyter
```

The notebooks are kept working on current library versions (pandas 2/3, NumPy 2,
scikit-learn 1.6, networkx 3.5, xgboost 3).

Notebook outputs are stripped from git via [nbstripout](https://github.com/kynan/nbstripout)
(see `.gitattributes`). After cloning, enable the filter once so your commits stay clean:

```bash
pip install nbstripout && nbstripout --install
```

## Data

CSVs live in `data/` and are loaded with a `data/...` relative path, so run Jupyter
from the repo root. One dataset ships compressed to keep the repo small — extract it
once before running Week 8:

```bash
cd data && unrar x "IMDB Dataset.rar"   # or: unar "IMDB Dataset.rar"
```

## Contents

| Notebook | Topic |
|-|-|
| Week 1 – Basics 1 | Python fundamentals: types, control flow, functions |
| Week 2 – Basics 2 | Files, iterators/generators, exceptions, string formatting |
| Week 3 – NumPy | Arrays, indexing, broadcasting, linear algebra |
| Week 4 – Pandas | Series/DataFrames, indexing, cleaning, missing data |
| Week 5 – Matplotlib | Figures/axes, common chart types, labels and legends |
| Week 6 – SciPy | Integration, interpolation, optimization, FFT |
| Week 7 – NetworkX | Graph construction, attributes, built-in algorithms |
| Week 8 – Regression & classification | scikit-learn: train/test split, metrics, baselines |
| Week 9 – XGBoost | Gradient boosting for regression and classification |
| EDA example | Worked exploratory analysis (Pima diabetes dataset) |

`exercises/` holds student worksheets for Weeks 1–6; `extras/` has supplementary demos.

## Google Colab

To run in Colab and access files from Drive, see
https://neptune.ai/blog/google-colab-dealing-with-files-2
