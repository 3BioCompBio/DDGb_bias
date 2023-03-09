
## Datasets

Datasets `S2536.csv` and `C380.csv` are our two main benchmark datasets. Predicted ΔΔGb values computed by the six predictors are assigned only for those two datasets.

### SKEMPI 2.0 [2] based datasets
- `SK2.csv` is the set of all mutations from SKEMPI 2.0 [2].
- `SK2_nr.csv` is the set of all non-redundant mutations from SKEMPI 2.0 that possess an assigned ΔΔGb value.
- `S4193.csv` is the set of all single mutations from `SK2_nr.csv`.
- `S2536.csv` is our first benchmark dataset of selected mutations from `S4193.csv`, which are mutations with a good resolution X-Ray crystallography PDB structure.

### CoV [3] based datasets
- `CoV.csv` is the set of all possible mutations from CoV [3] which mutated residue is contained in the PDB structure '6M0J'.
- `C380.csv` is the subset of mutations from `CoV.csv` located at the interface of the interaction.

## Notes
- Property `Entry` allow to relate each entry from a subset to corresponding initial entry or set of entries from its parent dataset. This can be useful in cases when multiple redundant entries (same mutation on same PDB) from `SK2.csv` generate a single entry in our benchmark dataset `S2536.csv`.
- Property `Mutation(s)` provide the residue and chain id of the mutation with respect to the SKEMPI 2.0 provided PDB while property `Mutation(s)_inPaper` provide the residue and chain id of the mutation with respect to the PDB from the Protein Data Bank.
- References are expressed as PuBMed-ids (when it exists).
- All properties ending with the suffix '_rev' concerns the reversed mutation on the mutated modeled PDB structure.
