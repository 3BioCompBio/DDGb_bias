
## Content

- `performances.ods`: Performance metrics (Pearson correlation, RMSE, shift, ...) of the six predictors on our two main benchmark datasets `S2536` and `C380`.
- `performances_subsets.ods`: Performance metrics of the six predictors on subsets of `S2536` (such as to alanine mutations vs. to non-alanine mutations).

## Notes about NetTree and discarded entries

Predictions of NetTree (one of the six studied predictors) failed on 16 entries from SK2536-D and SK2536-R for reasons that we were not able to identify. Thus, for fairness reasons and to keep the balance between the two datasets, we discarded those entries in both datasets (SK2536-D and SK2536-R) for all our benchmarks. The deletion of these few mutations leave the performances of other predictors almost unchanged and thus is considered as insignificant.
