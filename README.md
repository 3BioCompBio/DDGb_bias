
# Supplementary Data: Quantification of biases in predictions of protein-protein binding affinity changes upon mutations

## Description

Here are all the **Supplementary Data** related to the paper [1] (2023).

**Authors**: Matsvei Tsishyn, Fabrizio Pucci and Marianne Rooman.

## Conventions and units

- All energy values are in kcal/mol and all temperature values are in K.
- We use the convention that destabilizing mutations have positive ΔΔGb values.
- Separator in all `.csv` files is ';' and missing values are marked as 'XXX'. When a `.csv` cell's value represent a list, the elements are separated by ','.

## Content

### (1) Datasets

All mutations datasets referenced in the paper and all relative subsets can be found in `./1_datasets/` as well as additional mutations' properties (such as RSA, structural region, secondary structure and predicted ΔΔGb values).

### (2) Performances

All evaluations of the performances of the six predictors on `S2536` and `C380` as well as on subsets of `S2536` (such as to alanine mutations vs. to non-alanine mutations) can be found in `./performances/`.

### (3) Structures (wild-type and mutated)

Due to GitHub memory limitations, the PDB structures can not be stored here.
All wild-type and mutated PDB structures from datasets of mutations SKEMPI 2.0 [2] and CoV [3] are available at <http://babylone.3bio.ulb.ac.be/DDGb_bias_structures/>.
Mutated PDB structures are all modeled using comparative modeling software MODELLER [4] starting from its corresponding wild-type structure.

## References

  [1] Tsishyn, M., Pucci, F., & Rooman, M. (2023). Quantification of biases in predictions of protein-protein binding affinity changes upon mutations.

  [2] Jankauskaitė, J., Jiménez-García, B., Dapkūnas, J., Fernández-Recio, J., & Moal, I. H. (2019). SKEMPI 2.0: an updated benchmark of changes in protein–protein binding energy, kinetics and thermodynamics upon mutation. Bioinformatics, 35(3), 462-469.

  [3] Starr, T. N., Greaney, A. J., Hilton, S. K., Ellis, D., Crawford, K. H., Dingens, A. S., ... & Bloom, J. D. (2020). Deep mutational scanning of SARS-CoV-2 receptor binding domain reveals constraints on folding and ACE2 binding. cell, 182(5), 1295-1310.

  [4] Webb, B., & Sali, A. (2016). Comparative protein structure modeling using MODELLER. Current protocols in bioinformatics, 54(1), 5-6.
