# Gene Annotation Pipeline

## Steps

1. Organizing inputs: Naming genomes and RNAseq reads
2. Mapping RNAseq reads to the genome (STAR)
3. Calculating genome quality metrics (Assemblethon, BUSCOs) - seprate alt-haplotypes in genome, if any.
4. Remapping RNAseq reads to primary scaffolds/contigs only (STAR)
5. Running transcript assembly (Cufflinks, Strawberry, Stringtie, Class2 and Trinity), Splice junctions (Portcullis)
6. Run _ab initio_ gene prediction (BRAKER)
6. Map Trinity to genome to generate GFF3 (GMAP)
7. Pick transcripts for evidence-based predictions (Mikado)
8. Combine annotations (Mikado and Homology based predictions with _ab initio_) (GeMoMa)
9. Identify primary transcripts (TRaCE)
10. Finalize GFF3 files (custom)
11. Perform repeat annotations (EDTA)
12. Functional Annotations (TBD)

