
# Supplementary Data: Quantification of biases in predictions of protein-protein binding affinity change upon mutations


## (1) Description
Here are all the Supplementary Data related to the paper [1] (2023).

Authors: Matsvei Tsishyn, Fabrizio Pucci and Marianne Rooman.  
Université Libre de Bruxelles, 3BIO-CompBio, Computational Biology and Bioinformatics.


## (2) Conventions and units
- All energy values are in kcal/mol and all temperature values are in K.
- We use the convention that destabilizing mutations have positive ΔΔGb values.
- Separator in all `.csv` files is ';' and missing values are marked as 'XXX'. When a `.csv` cell's value represent a list, the elements are separated by ','.


## (3) Content
For additional information and precisions, each data-folder contains its own `README.md`.

### (3.1) Datasets
All mutations datasets referenced in the paper and all relative subsets can be found in `./1_datasets/` as well as additional mutations' properties (such as RSA and predicted ΔΔGb values).

### (3.2) Predictors' main training datasets
The main training datasets of the predictors mCSM-PPI2, MutaBind2, BeAtMuSiC, SSIPe and NetTree can be found in `./2_predictors_datasets/`.

### (3.3) Performances
All evaluations of the performances of the six predictors on `S2536` and `C380` as well as on subsets of `S2536` (such as to alanine mutations vs. to non-alanine mutations) can be found in `./performances/`.

### (3.4) Structures (wild-type and mutated)
NOTE: Due to GitHub memory limitations, the PDB structures can not be stored here.  
All wild-type and mutated PDB structures from datasets of mutations SKEMPI 2.0 [2] and CoV [3] are available at  http://babylone.3bio.ulb.ac.be/DDGb_bias_structures/.  
The wild-type structure '6M0J' used in CoV comes directly from the Protein Data Bank (https://www.rcsb.org/structure/6M0J).  
All other wild-type structures from SKEMPI 2.0 are the one provided by SKEMPI 2.0's authors (rather than from the Protein Data Bank) since they are curated to be as close as possible to the experimental measures of the dataset. Additionally, we corrected some errors in a few PDB structures (as mentioned in the paper [1]).  
Mutated PDB structures are all modeled using comparative modeling software MODELLER [4] starting from its corresponding wild-type structure.

### (3.5) Mutually-reversed complexes (mutations)
All pairs of mutually-reversed complexes and related information can be found in `./mutually_reversed_mutations/`.


## (4) References
  [1] Tsishyn, M., Pucci, F., & Rooman, M. (2023). Quantification of biases in predictions of protein-protein binding affinity change upon mutations.

  [2] Jankauskaitė, J., Jiménez-García, B., Dapkūnas, J., Fernández-Recio, J., & Moal, I. H. (2019). SKEMPI 2.0: an updated benchmark of changes in protein–protein binding energy, kinetics and thermodynamics upon mutation. Bioinformatics, 35(3), 462-469.

  [3] Starr, T. N., Greaney, A. J., Hilton, S. K., Ellis, D., Crawford, K. H., Dingens, A. S., ... & Bloom, J. D. (2020). Deep mutational scanning of SARS-CoV-2 receptor binding domain reveals constraints on folding and ACE2 binding. cell, 182(5), 1295-1310.

  [4] Webb, B., & Sali, A. (2016). Comparative protein structure modeling using MODELLER. Current protocols in bioinformatics, 54(1), 5-6.
