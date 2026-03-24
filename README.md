# 2D-Membrane-Desalination-Data
Accelerating Water Desalination Screening of 2D Membranes via Machine Learning Surrogates
This repository presents a **data-driven framework for accelerating water desalination research** by replacing expensive molecular dynamics (MD) simulation cycles with a fast surrogate machine learning pipeline. The project focuses on predicting the desalination performance of **2D membrane materials** using membrane- and pore-level physicochemical features.

The two main prediction targets are:
- **Water flux**
- **Ion rejection**

By learning from previously generated MD simulation data, this workflow enables faster screening of candidate nanomembranes and helps identify promising designs for reverse osmosis and related water treatment applications.

The repository includes:
- a **desalination dataset** (Desalination_updated_Nov09.csv) with membrane and simulation-related features,
- a **Jupyter notebook** for exploratory analysis and model benchmarking,
- a workflow for evaluating how individual features relate to **ion rejection**,
- and visualizations comparing **permeation rate** and **salt rejection** across membrane technologies.

This figure visual summarizes the entire value proposition: turning complex Molecular Dynamics (MD) into fast Machine Learning insights.

<img width="1408" height="768" alt="image" src="https://github.com/user-attachments/assets/3aabe9c0-23f1-4d26-8e42-645c35cd803e" />


From the uploaded dataset, the current tabular data includes the following columns:
- `Area`
- `Pressure`
- `Sigma1`
- `Epsilon1`
- `Sigma2`
- `Epsilon2`
- `Thickness`
- `Flux`
- `Rejection`
- `Materials`

The dataset spans a range of membrane/system conditions and uses **Flux** and **Rejection** as the primary outputs.


## Getting started

### Requirements
Typical Python packages used in the notebook include:
- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost

Install them with:

```bash
pip install pandas numpy matplotlib scikit-learn xgboost
```

### Run the notebook

```bash
water_desalination-jan11.ipynb
```

---

## Notes

The uploaded notebook references feature names such as `e1`, `e2`, and `thickness`, while the uploaded CSV currently uses `Epsilon1`, `Epsilon2`, and `Thickness`. If needed, align the column names before running the notebook end-to-end.

---

## Research motivation

This project is motivated by the need to reduce the time and energy costs of desalination-performance evaluation. By combining MD-generated data with surrogate machine learning models, the framework supports a more scalable route for studying and optimizing nanomaterial membranes for water treatment.

The broader goal is to move from **slow simulation-only evaluation** toward **fast, data-guided screening and design**.
