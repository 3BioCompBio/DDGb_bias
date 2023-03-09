
## Contents
Here are the main training datasets the predictors mCSM-PPI2, MutaBind2, BeAtMuSiC, SSIPe and NetTree. Those datasets come respectively from the original paper of its predictor. For the sake of simplicity, we standardized all the datasets in the same syntax.

## Note about SAAMBE-3D
Main training dataset of SAAMBE-3D is not specified in its original paper. However it is stated that it is derived from single mutations of SKEMPI 2.0 and contains 3753 entries. When estimating how many entries from S2536 where known by SAAMBE-3D, we used the fact than SAAMBE-3D kept a fraction of 0.90 (=3753/4193) of all single mutations from SKEMPI 2.0. We supposed the independence between our selection criteria (good resolution of the structure) and SAAMBE-3D criteria (small ΔΔGb variance of the redundencies and no missing residues close to the mutation) to extimate that SAAMBE-3D known 0.90 of entries from S2536. This value is close to the real fraction as it is necessary contained between 0.83 and 1.0 (supposing extreme cases when all or none values excluded by SAAMBE-3D are in S2536).
