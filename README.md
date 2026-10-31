# Machine Learning Assignment 2 — Olivetti Faces


## Main file

- `ML_assignment_2.ipynb` — original Jupyter notebook containing the student's work for the assignment.

## Dataset and generated files

The notebook loads the Olivetti Faces dataset using `sklearn.datasets.fetch_olivetti_faces()`. The dataset may be downloaded by scikit-learn on first execution, so internet access may be required unless it is already cached locally.

The notebook writes `olivetti_split.npz` when its split-generation cell is executed. This generated file is not included in this starter package because it was not present alongside the uploaded notebook at packaging time. After running the notebook, retain the generated file in the repository if the assignment requires the split indices to be submitted.

## Repository folders

- `figures/` — The exported figures here.
- `logs/` — The final execution log or captured results here after running the notebook.
- `configs/` — For configuration files.

## Environment

The notebook uses Python packages including NumPy, pandas, Matplotlib, and scikit-learn. See `requirements.txt` for an installable dependency list. It is a compatibility-oriented list, not a record of the exact package versions installed on the original machine. For strict environment reproduction, create a lock file from the environment in which the notebook is successfully run.




