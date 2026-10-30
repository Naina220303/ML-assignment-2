# Configurations

`experiment_config.json` records the dataset, stratified split, random seeds, model hyperparameters, ensemble sizes, masking settings, repetition counts, and evaluation settings extracted from `ML_assignment_2.ipynb`.

## Source of truth

The original notebook remains the source of truth. This file documents the settings as written; it does not modify the notebook, fix implementation issues, or claim that the experiments have been independently rerun.

## Notes

- JSON `null` for a tree depth corresponds to `max_depth=None` in scikit-learn.
- Q3(a) uses 5 repetitions. Q3(b) uses 3 repetitions, and Q3(c) and Q3(d) reuse the Q3(b) resamples.
- The exact installed package versions are not recorded here; see the repository's environment/reproduction instructions for how to capture them after a successful run.
