Column Name: Description

To quantify mRNA stability, we use a ratio of ratios, comparing the expression 4 h after the addition of Dox (t4) to the steady-state expression (t0):
*** t4/t0 = mRNA stability

SNP: SNPs contained within the 160nt sequence segment.

hap: Haplotype encoded in this sequence segment.  0s and 1s correspond to reference and alternate alleles; mutated_ARE, mutated_CDE, etc. correspond to deliberate mutations

ids: A name for the sequence segment.

overlapWith: Gives a list of elements the sequence segment overlaps with.

overlapWithAndSNPInside: Gives a list of elements the sequence segment overlaps with and which a SNP in the oligo overlaps.

region: Takes the form GENE|CHROM:START-END.

seq: The sequence of the segment.

iscontrol: 1 if reference; 0 if a deliberate mutation or alt allele

parent_control_oligo: The id of the reference segment for a deliberate mutation or alt allele (its own id if it is a reference).

issnp: 1 if it is a SNP, 0 otherwise

GC_content: Fraction of GC.

ratios_T0: RNA/(RNA+DNA) at T0 for the sequence segment (summing over all clones for RNA and DNA)

ratios_T4T0: ratios_T4/(ratios_T4+ratios_T0)

ratios_T0_GC_resid: ratios_T0 after residualizing with respect to GC (better to use this)

*** ratios_T4T0_GC_resid: ratios_T4T0 after residualizing with respect to GC (better to use this) ***

effect_size_T0: Difference in ratios_T0 between reference and alt/mutant (sign is alt/mutant minus reference)

effect_size_T4T0: Difference in ratios_T4T0 between reference and alt/mutant (sign is alt/mutant minus reference)

effect_size_T0_GC_resid: effect_size_T0 after residualizing by GC (better to use this but difference is small)

effect_size_T4T0_GC_resid: effect_size_T4T0 after residualizing by GC (better to use this but difference is small)

one_ARE_deleted: 1 if exactly 1 ARE was deliberately mutated, 0 otherwise

top_ARE_deleted: 1 if the mutated ARE was the longest ARE in the sequence segment, 0 otherwise

motif_AREs_numbered_BakheetPlus: ARED-Plus "cluster" number.  -1 if no ARE, 0 if ARE smaller than ARED-Plus clusters but larger than "AUUUA".

ARE_registration_perfect: Registration of the ARE, assuming perfect match to AUUUA motif with no mismatches (integer value, nan if no ARE present).

ARE_length_perfect: Length of the ARE, assuming perfect match to AUUUA motif with no mismatches (integer value, nan if no ARE present).

CDE_stem_lengths: Length of the lower CDE stem.  -1 means no CDE; 0 (or 1) means there is no lower stem but the motif exists.

parent_CDE_stem_length: If hap=='mutated_CDE', this is the length of the lower CDE stem of the parent (corresponding un-mutated) sequence.

ratios_T2T0: ratios_T2/(ratios_T2+ratios_T0)

ratios_T2T0_GC_resid: ratios_T2T0 after residualizing with respect to GC (better to use this)

effect_size_T2T0: Difference in ratios_T2T0 between reference and alt/mutant (sign is alt/mutant minus reference)

effect_size_T2T0_GC_resid: effect_size_T2T0 after residualizing by GC (better to use this but difference is small)

ratios_T6T0: ratios_T6/(ratios_T6+ratios_T0)

ratios_T6T0_GC_resid: ratios_T6T0 after residualizing with respect to GC (better to use this)

effect_size_T6T0: Difference in ratios_T6T0 between reference and alt/mutant (sign is alt/mutant minus reference)

effect_size_T6T0_GC_resid: effect_size_T6T0 after residualizing by GC (better to use this but difference is small)

parent_motif_AREs_numbered_BakheetPlus: For mutated AREs, this is the ARED-Plus "cluster" number of the "parent" ARE.
