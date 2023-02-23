
# DDGb_bias-supplementary_materials


## (1) Introduction
Here are all supplementary data for the paper [1].


## (2) Conventions and units
- All energy values are in kcal/mol and all temperature values are in K.
- We use the convention that destabilizing mutations have positive ΔΔGb values.
- Separator in all .csv files is ";" and missing values are marked as "XXX".
- When a .csv cell's property represent a list, the elements are separated by ",".


## (3) Content

### (3.1) Datasets
All mutations dataset referenced in the paper and all generated subsets are uniformed in the same syntax and can be found in `./datasets/`.
All additionally computed mutation's properties are also added to those files.

### (3.2) Performances
All evaluations of the performances of the six predictors can be found in `./performances/`.

### (3.3) Structures
All wild-type and mutated PDB structures are available to download here: http://babylone.3bio.ulb.ac.be/DDGb_bias_structures/
We also modelled (with MODELLER) all mutated PDB structures for all mutations from [2] and [3]
(including mutations on which we did not tested the predictors).

### (3.4) Mutually-reversed complexes (mutations)
All pairs of mutually-reversed complexes and related information can be found in `./mutually_reversed_mutations/`.


## (4) References
  [1] Tsishyn, M., Pucci, F., Rooman, M (2023). DDGb bias paper.

  [2] Jankauskaitė, J., Jiménez-García, B., Dapkūnas, J., Fernández-Recio, J., & Moal, I. H. (2019). SKEMPI 2.0: an updated benchmark of changes in protein–protein binding energy, kinetics and thermodynamics upon mutation. Bioinformatics, 35(3), 462-469.

  [3] Starr, T. N., Greaney, A. J., Hilton, S. K., Ellis, D., Crawford, K. H., Dingens, A. S., ... & Bloom, J. D. (2020). Deep mutational scanning of SARS-CoV-2 receptor binding domain reveals constraints on folding and ACE2 binding. cell, 182(5), 1295-1310.
