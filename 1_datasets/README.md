
# Datasets

Datasets `S2536.csv` and `C380.csv` are our two main benchmark datasets. Predicted ΔΔGb values computed by the eight predictors are assigned only for those two datasets.

## SKEMPI 2.0 based datasets

- `SK2.csv` is the set of all mutations from SKEMPI 2.0 [2] with assigned ΔΔGb value.
- `SK2_nr.csv` is the subset of non-redundant mutations from `SK2.csv`.
- `S4193.csv` is the subset of single mutations from `SK2_nr.csv`.
- `S2536.csv` is the subset of mutations from `S4193.csv` with a good resolution X-Ray crystallography PDB structure.

## CoV based datasets

- `C3684.csv` is the set of all mutations from CoV [3] which mutated residue is contained in the PDB structure '6M0J'.
- `C380.csv` is the subset of mutations from `C3684.csv` located at the interface of the interaction.

## SK2_sym: Mutually reversed complexes from SKEMPI 2.0

- `SK2_sym.csv` is set of pairs of complexes from SKEMPI 2.0 that are separated by a single mutation.
- **WARNING**: **Some of the pairs of complexes have more differences than a single mutation** such as the presence of a modified amino acid, some missing residues or additional mutation(s) far from the interface. Such differences are specified in the dataset.
To help the reader to locate and specify the nature of those differences, chain-by-chain alignments of similar complexes are provided in `SK2_sym_alignments.zip`. The alignments are done on SEQRES lines of the PDB.

## Notes

- Property `Entry` allows to link each entry from a subset to its corresponding initial entry or set of entries from its parent dataset. This can be useful in cases when multiple redundant entries (same mutation on same PDB) from `SK2.csv` generate a single entry in our benchmark dataset `S2536.csv`.
- Property `Mutation(s)` provides the residue and chain id of the mutation with respect to the PDB provided by SKEMPI 2.0, while property `Mutation(s)_in_raw_pdb` provides the residue and chain id of the mutation with respect to the "raw" PDB from the Protein Data Bank.
- References are expressed as PuBMed-ids (when it exists).
- All properties ending with the suffix `_rev` concern the reverse mutation on the mutated modeled PDB structure.
