# Arntor – Computational Genomics Toolkit

This project is a modular computational genomics toolkit designed to analyze genomic structure at multiple biological scales.

It integrates:
- DNA-level repeat region classification (STRs)
- RNA-level transcript structure annotation

## Motivation

Genomic regulatory architecture is inherently multi-scale. While repetitive DNA elements (STRs) affect genome stability and regulation, transcript-level structures determine gene expression complexity.

This toolkit was developed to provide a unified computational framework for analyzing both levels using standard bioinformatics tools.

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
