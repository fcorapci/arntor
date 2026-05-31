# arntor
Arntor is a command-line tool that classifies short tandem repeats (STRs) into genomic regions such as promoters, exons, introns, and intergenic regions.

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
