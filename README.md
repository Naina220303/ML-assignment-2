# Machine Learning Assignment 2 — Olivetti Faces

This repository packages the **original notebook supplied by the student**. The notebook has been copied without editing its code, cell order, parameters, outputs, or experimental settings.

## Main file

- `ML_assignment_2.ipynb` — original Jupyter notebook containing the student's work for the assignment.

## Dataset and generated files

The notebook loads the Olivetti Faces dataset using `sklearn.datasets.fetch_olivetti_faces()`. The dataset may be downloaded by scikit-learn on first execution, so internet access may be required unless it is already cached locally.

The notebook writes `olivetti_split.npz` when its split-generation cell is executed. This generated file is not included in this starter package because it was not present alongside the uploaded notebook at packaging time. After running the notebook, retain the generated file in the repository if the assignment requires the split indices to be submitted.

## Repository folders

- `figures/` — place exported figures here if required.
- `logs/` — place the final execution log or captured results here after running the notebook.
- `configs/` — reserved for configuration files if you decide to export them separately. No configuration has been invented or extracted into a new format.

## Environment

The notebook uses Python packages including NumPy, pandas, Matplotlib, and scikit-learn. See `requirements.txt` for an installable dependency list. It is a compatibility-oriented list, not a record of the exact package versions installed on the original machine. For strict environment reproduction, create a lock file from the environment in which the notebook is successfully run.

## Run the notebook

See [`reproduction_commands.md`](reproduction_commands.md). Run all cells in order in Jupyter. Save the executed notebook and generated split after confirming that the run completes successfully.

## Before submission

Add the actual GitHub repository URL, student name, roll number, and final commit hash to the paper/report wherever required. Obtain the URL and hash from your own GitHub repository after pushing; do not use placeholders as final submission details.

## Integrity note

This package intentionally does not correct or reinterpret the notebook. Any questions about the methodology or results should be discussed separately, with the original notebook remaining unchanged unless the student explicitly requests an edit.
