# arntor
Arntor is a lightweight computational genomics tool designed to classify short tandem repeats (STRs) into functional genomic regions using gene annotations and repeat element data. It integrates standard bioinformatics tools (bedtools, TRF) into a reproducible analysis pipeline.

## What it does

- Takes genome annotation (GTF file)
- Takes STR data (TRF output)
- Matches STRs to genomic regions using bedtools
- Outputs classified STR regions

## Requirements

- bash
- bedtools
- awk

## Usage

```bash
./arntor annotation.gtf trf.tsv chrom.sizes prefix upstream downstream
