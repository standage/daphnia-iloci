```bash
# Add correct `##sequence-region` pragmas to GFF3 file.
time seq-reg.py FrozenGeneCatalog20110204.gff3 Daphnia_pulex.fasta > Dpul.gff3

# Compute iLoci (lpdriver.py runs LocusPocus)
time lpdriver.py --namefmt=DpulILC-%06lu --out=Dpul.iloci.gff3 Dpul.gff3

# Drosophila data prepared with GenHub

# All other processing done in the Jupyter notebook
```
