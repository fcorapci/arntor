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

## Workflow

1. Parse gene annotation (GTF)
2. Extract genomic features (exons, promoters, introns)
3. Process STR coordinates (TRF output)
4. Intersect STRs with genomic regions using bedtools
5. Output region-specific STR classifications

## Usage

```bash
./arntor annotation.gtf trf.tsv chrom.sizes prefix upstream downstream
