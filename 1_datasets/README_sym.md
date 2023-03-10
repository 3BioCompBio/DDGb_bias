
# Set of mutually reversed complexes

## Introduction

Here we define the dataset of all pairs of complexes that are separated by exactly
one single mutation, such as:

           -----TI39P---> (ΔΔGb = +3.754)
  1TM1_E:I <------------> 1Y33_E:I
           <----PI39T---- (ΔΔGb = -3.754)

We then say that 1TM1_E:I_TI39P and 1Y33_E:I_PI39T are "mutually reversed".

## WARNING

(1) Some of the mutually reversed pairs of complexes are not included in SKEMPI 2.0 and thus
do not have any associated ΔΔGb values. These entries can not be used to train a ΔΔGb predictor,
however they can be used as a test set to verify if the predictor is able to satisfy
the symmetry relation: ΔΔGb(A->B) + ΔΔGb(B->A) = 0

(2) Some of the mutually reversed pairs of complexes contains other minor differences including:
  - usage of non-standard amino acids in only one of the two complexes
  - missing amino acids in the tails (C- and N-terminus) of a chain
  - insertion/delete in the middle of a chain
  - additional mutations that are far from the interface (and that may be, in some cases, considered as negligible)
  - inversion of two amino-acids in the tail of a chain
The presence of such additional differences in a pair is specified in the dataset.
We tried to be loose and keep pairs containing such differences in the dataset,
however WE STRONGLY ADVISE THE READER TO FILTER THE DATASET depending on the context
before using it for training or testing.

## Content

(1) "SK2_sin_mutually-reversed.csv" is the dataset of mutually reversed pairs of complexes.
The separator is ";" and when a property's value is missing, it is marked as "XXX".
When multiple different sources report a ΔΔGb for the direct or/and the reversed mutation, we
average the ΔΔGb value (taking into account the change of the sign).
The presence of additional differences between the complexes are specified in the
properties "tail_gaps", "internal_gaps", "other_mutations" and "WARNING" and we advise
the readers to pay attention to these properties.

(2) For each pair of mutually reversed complexes, we provide the chain-by-chain, sequence-identity alignment
(in "SK2_sin_mutually-reversed_align.zip") so that the location and the nature of the differences
between the two complexes can be easily located.
The alignment is performer on the SEQRES lines of the PDB.
