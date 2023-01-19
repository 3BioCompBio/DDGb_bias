
# DDGb_bias-supplementary_materials

## (1) Introduction
Here are all supplementary data for DDGb bias paper [1].

## (2) Conventions and units
- All energy values are in kcal/mol and all temperature values are in K.
- By convention, destabilizing mutations have positive ΔΔGb values.
- Separator in all .csv files is ";" and missing values are marked as "XXX".

## (3) Content

### (3.1) Datasets
- `./datasets/PDB.csv` contains some summary information about all used PDB structures in the paper.
- `./datasets/SK2.csv` is the set of all mutations from SKEMPI 2.0 [2].
- `./datasets/SK2_nr.csv` is the set of all non-redundant mutations from SKEMPI 2.0 that possess an assigned a ΔΔGb value.
- `./datasets/SK2_single.csv` is the set of all single mutations from `SK2_nr`.
- `./datasets/S2536.csv` is our dataset of selected mutations from `SK2_single` (mutations with a good resolution X-Ray crystallography structure).
- `./datasets/S2536_balanced.csv` is a subset of `S2536` balanced by mutation type (only 5 random mutations are kept by mutation type).
- `./datasets/CoV.csv` is the set of all possible mutations on the PDB structure 6M0J studied in [3].
- `./datasets/C380.csv` is the subset of mutations from `CoV` with an assigned ΔΔGb values and located at the interface of the interaction.
- Predicted values obtained by the six predictors for direct and reverse mutations are computed only for the datasets `S2536` and `C380`.

### (3.2) Results
- All statistics about the performances of the predictors are in `./statistics/performances.ods`.
- All statistics about the performances of the predictors on S2536-D when partitioned in subsets are in `./statistics/performances_subsets.ods`.

### (3.3) Structures
All wild-type and mutated PDB structures are available here: http://babylone.3bio.ulb.ac.be/DDGb_bias_structures/


## (4) References
  [1] Tsishyn, M., Pucci, F., Rooman, M (2023). DDGb bias paper.

  [2] Jankauskaitė, J., Jiménez-García, B., Dapkūnas, J., Fernández-Recio, J., & Moal, I. H. (2019). SKEMPI 2.0: an updated benchmark of changes in protein–protein binding energy, kinetics and thermodynamics upon mutation. Bioinformatics, 35(3), 462-469.

  [3] Starr, T. N., Greaney, A. J., Hilton, S. K., Ellis, D., Crawford, K. H., Dingens, A. S., ... & Bloom, J. D. (2020). Deep mutational scanning of SARS-CoV-2 receptor binding domain reveals constraints on folding and ACE2 binding. cell, 182(5), 1295-1310.
