# Arntor – Computational Genomics Toolkit

Arntor is a computational genomics toolkit that integrates DNA-level and RNA-level genomic annotation pipelines.

It provides modular tools for structural classification of genomic features using standard bioinformatics frameworks.

---

## Tools

### 1. arntor
Classifies short tandem repeats (STRs) into functional genomic regions (promoter, exon, intron, intergenic) using genome annotations and repeat data.

**Promoter definition:**
By default, promoter regions are defined as ±1000 bp around transcription start sites (TSS). This window is configurable via command-line arguments.

---

### 2. regionbytranscript
Extracts exon and intron structures from GTF files and assigns transcript-level intron ordering using Bioconductor (GenomicFeatures).

---

## Requirements

- bash
- R (GenomicFeatures, dplyr)
- bedtools
- awk

---

## Usage

### arntor
```bash
arntor annotation.gtf trf.tsv chrom.sizes prefix 1000 1000
```
### regionbytrancsript
```bash
regionbytranscript annotation.gtf hg38 output_dir hg38_chrom.sizes
```
