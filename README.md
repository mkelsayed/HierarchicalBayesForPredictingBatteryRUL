# HierarchalBayesForPredictingBatteryRUL

## Environment Setup

Two conda environments are used in this project — one for preprocessing and EDA and another for modeling.

**Preprocessing and EDA:**
```bash
conda env create -f environment_preprocessing_EDA.yml
conda activate 
```

**Modeling:**
```bash
conda env create -f environment_analysis.yml
conda activate 
```

The first three notebooks mentioned below can run on the first environment. The fourth notebook runs on the second environment.


## Data Acquisition

We aquired data from 2 sources: 
- https://data.matr.io/1/projects/5c48dd2bc625d700019f3204 (all datasets)
- https://data.matr.io/1/projects/5d80e633f405260001c0b60a (only batch 9)

Place it in a folder called `data/` then run the notebooks in the following order.

## Order of Notebooks

- `matlabToPickle.ipynb`
- `dataCleaning.ipynb`
- `EDA.ipynb`
- `Analysis.ipynb`

## Outline of Report

* Introduction
* Background
* Data Overview
  * Data Structure and Extraction
  * Data Partitioning and Grouping Logic
  * Grouping Results
* Introduction to Hierarchical Bayes
  * Multilevel Modelling
  * Pooling Tradeoff
  * Pooling Tradeoff: County Radon Levels
  * Partial Pooling
  * Hierarchical Bayes
* Hierarchical Bayesian Model for Battery Lifetime Prediction 
  * Model Details 
  * Inference
* Conclusion
