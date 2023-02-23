
## Content

- `PDB.csv` contains some summary information about all used PDB structures in the paper.
- `SK2.csv` is the set of all mutations from SKEMPI 2.0 [2].
- `SK2_nr.csv` is the set of all non-redundant mutations from SKEMPI 2.0 that possess an assigned a ΔΔGb value.
- `SK2_single.csv` is the set of all single mutations from `SK2_nr`.
- `S2536.csv` is our dataset of selected mutations from `SK2_single` (mutations with a good resolution X-Ray crystallography structure).
- `S2536_balanced.csv` is a subset of `S2536` balanced by mutation type (only 5 random mutations are kept by mutation type).
- `CoV.csv` is the set of all possible mutations on the PDB structure 6M0J studied in [3].
- `C380.csv` is the subset of mutations from `CoV` with an assigned ΔΔGb values and located at the interface of the interaction.
- Predicted values obtained by the six predictors for direct and reverse mutations are computed only for the datasets `S2536` and `C380`.
