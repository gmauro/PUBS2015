# Data Generation #

The file and path names in this document may differ slightly from those in this project. The software package ART is used to generate several of the data sets:

http://www.niehs.nih.gov/research/resources/software/biostatistics/art/

## Escherichia coli O104:H4 str. 2011C-3493 plasmid pESBL-EA11 ##

Accession: NC_018659.1

http://www.ncbi.nlm.nih.gov/nuccore/NC_018659.1

Reads generated with ART:

./art_illumina -i Ecoli_O104H4_pESBL.fasta -l 250 -f 30 -qs 10 -qs2 10 -o Ecoli_O104H4_pESBL

## Clostridium botulinum A str. ATCC 3502 plasmid pBOT3502 ##

Accession: NC_009496.1

http://www.ncbi.nlm.nih.gov/nuccore/NC_009496.1

Reads generated with ART:

./art_illumina -i Cbotulinum_A_pBOT3502.fasta -l 250 -f 30 -qs 10 -qs2 10 -o Cbotulinum_A_pBOT3502

## Rhodobacter sphaeroides 2.4.1 chromosome 1 ##

Source: GAGE Genome Project

http://gage.cbcb.umd.edu/data/Rhodobacter_sphaeroides/Data.original/

Reads generated by converting to FASTQ format and performing a simple data reduction:

head -n 20000 frag_1.fastq > unknown.fastq

## UNKNOWN: Mycoplasma mycoides subsp. mycoides SC str. PG1 chromosome ##

Accession: NC_005364.2

http://www.ncbi.nlm.nih.gov/nuccore/NC_005364.2

Reads generated with ART:

./art_illumina -i MycoplasmaMycoides.fasta -l 250 -f 5 -qs 10 -qs2 10 -o unknown