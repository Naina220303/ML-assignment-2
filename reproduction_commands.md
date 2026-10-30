# Reproduction commands (Windows / Anaconda Prompt)

These commands are a starting point for running the notebook as supplied. They do not modify the notebook's code or experimental settings.

## 1. Create and activate an environment

```bat
conda create -n ml-assignment python=3.10 -y
conda activate ml-assignment
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## 2. Launch Jupyter

```bat
jupyter lab
```

Open `ML_assignment_2.ipynb` and use **Kernel → Restart Kernel and Run All Cells**. The first run may need internet access to download the Olivetti Faces dataset through scikit-learn.

## 3. Save reproducibility artifacts

After a successful run, check whether `olivetti_split.npz` was created in the notebook's working directory. Keep that file with the submission if the assignment asks for saved split indices. Save the executed notebook separately so the original notebook remains unchanged:

```bat
jupyter nbconvert --to notebook --execute ML_assignment_2.ipynb --output executed_ML_assignment_2.ipynb
```

If the notebook was already executed interactively, save it from Jupyter as well. Capture final outputs/logs in `logs/` and export any required figures to `figures/`.

## 4. Record the exact environment after a successful run

```bat
python --version
pip freeze > requirements-lock.txt
```

`requirements-lock.txt` records the package versions in the environment actually used. Commit it if exact environment reproduction is required.

## 5. Push to GitHub

Create an empty GitHub repository first, then run these commands from this folder (replace the branch/remote details only if your GitHub setup differs):

```bat
git init
git add .
git commit -m "Add original ML Assignment 2 notebook"
git branch -M main
git remote add origin YOUR_GITHUB_REPOSITORY_URL
git push -u origin main
git rev-parse HEAD
```

Copy the actual repository URL and commit hash printed by the last command into the report.

## Important

The original notebook is intentionally preserved as supplied. These instructions do not assert that every cell has been independently re-executed in this packaging environment. Confirm a successful full run on your computer before describing the repository as fully reproduced.
