# Applied Machine Learning

Companion examples for the book **Applied Machine Learning** by Bahareh Rahmani.

This repository presents the book's Python examples as a practical introduction to
machine-learning workflows. The material progresses from Python fundamentals and
data visualization to feature selection, supervised learning, clustering, and
ensemble methods. Explanations, dataset context, and reported results remain tied
to the corresponding examples in the book.

## Contents

| Chapter | Topic | Example data |
| ---: | --- | --- |
| 1 | [Python fundamentals](chapters/chapter-01-python-basics/python-basics.ipynb) | USDA rural-development borrowers |
| 2 | [Loading and visualizing data](chapters/chapter-02-data-visualization/data-visualization.ipynb) | Iris and USDA data |
| 3 | [Feature selection](chapters/chapter-03-feature-selection/feature-selection.ipynb) | Forest Fires |
| 4 | [Linear and logistic regression](chapters/chapter-04-regression/regression.ipynb) | Pokemon |
| 5 | [Multiclass logistic regression](chapters/chapter-05-multiclass-logistic-regression/multiclass-logistic-regression.ipynb) | Forest Fires |
| 6 | [Decision trees](chapters/chapter-06-decision-trees/decision-trees.ipynb) | Social Media vs Productivity |
| 7 | [K-nearest neighbors](chapters/chapter-07-k-nearest-neighbors/knn-classification.ipynb) | Depression and Anxiety |
| 8 | [Support-vector machines](chapters/chapter-08-support-vector-machines/svm-classification.ipynb) | Flight Price Prediction |
| 9 | [K-means clustering](chapters/chapter-09-k-means-clustering/k-means-clustering.ipynb) | Worldwide Temperature |
| 10 | [Hierarchical clustering](chapters/chapter-10-hierarchical-clustering/hierarchical-clustering.ipynb) | NYC Air Quality |
| 11 | [XGBoost and random forests](chapters/chapter-11-ensemble-methods/ensemble-methods.ipynb) | Pima Diabetes and Iris |

The original collected examples are preserved in [Codes.pdf](Codes.pdf). The code
is organized into chapter-level Jupyter notebooks so readers can work through each
example independently while comparing it with the published material.

## Repository principles

- Preserve the scientific methods, feature choices, and reported results from the
  book.
- Keep the original source material unchanged.
- Document compatibility corrections separately from methodological changes.
- Make each chapter self-contained where practical.
- Record dataset provenance, licensing, and any preprocessing needed to reproduce
  an example.
- Do not place credentials, private information, or unapproved datasets in version
  control.

## Getting started

The chapter notebooks are available above. The dependency manifest is being
prepared from the original material; the intended local workflow is:

```bash
python -m venv .venv
```

Activate the environment on macOS or Linux:

```bash
source .venv/bin/activate
```

Activate it on Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

Then install the dependencies and launch JupyterLab:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Python dependencies used by the examples include NumPy, pandas, Matplotlib,
SciPy, scikit-learn, XGBoost, and Graphviz. Graphviz may also require a separate
system installation.

## Data

Datasets are not bundled by default. Readers should obtain them from their original
publishers and follow the preparation instructions supplied with the relevant
chapter. This keeps the repository small and respects source-specific licensing,
attribution, and ethical-use requirements.

Primary sources used by the book examples include:

- [USDA Section 502 borrower data](https://catalog.data.gov/dataset/usda-rural-development-single-family-section-502-direct-active-borrowers-by-county)
- [UCI Forest Fires](https://archive.ics.uci.edu/dataset/162/forest)
- [The Complete Pokemon Dataset](https://www.kaggle.com/datasets/rounakbanik/pokemon)
- [Social Media vs Productivity](https://www.kaggle.com/datasets/mahdimashayekhi/social-media-vs-productivity)
- [Depression and Anxiety Data](https://www.kaggle.com/datasets/shahzadahmad0402/depression-and-anxiety-data)
- [Flight Price Prediction](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)
- [Temperature of All Countries](https://www.kaggle.com/datasets/subhamjain/temperature-of-all-countries-19952020)
- [NYC Air Quality and Health Impacts](https://catalog.data.gov/dataset/air-quality)
- [Pima Diabetes](https://www.kaggle.com/datasets/mathchi/diabetes-data-set)

The Iris dataset is loaded directly through scikit-learn.

Some chapters use health or behavioral data. These examples are provided solely
for education and are not intended for medical diagnosis, treatment, or decisions
about individuals.

## Reproducibility

Some examples in the original material use randomized train/test splits or model
initialization without a fixed random seed. Results can therefore vary between
runs and library versions. The repository will distinguish the results printed in
the book from newly generated notebook output.

Corrections needed only for modern library compatibility will be documented in the
relevant chapter. Changes that could alter the methodology or reported conclusions
will not be made silently.

## Contributing

Corrections that improve clarity, portability, or reproducibility are welcome.
Please describe whether a proposed change affects only presentation or runtime
compatibility, or whether it changes the scientific method or results.

## Citation

If you use these examples in teaching, research, or another publication, please
cite **Applied Machine Learning** and this repository. Complete bibliographic and
machine-readable citation details will be added when the book's publication
metadata is finalized.

## License

No software license has been selected yet. Unless a `LICENSE` file is added, the
code and documentation remain protected by copyright and no reuse license is
granted. Referenced datasets retain their own licenses and terms of use.
