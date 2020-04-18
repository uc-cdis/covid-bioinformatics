# covid-bioinformatics
Software tools to collect and analyze Coronavirus sequences, including code to create gene and protein entries 
starting with COV (coronavirus) genome files downloaded from NCBI, then create gene and protein-specific 
collections, alignments, and HMMs.

Typical usage:

*./download-gb-by-taxid.py*

*./feature-to-gene-and-protein.py *.gb*

*./seqs-to-aligns-and-hmms.py *.fasta*

The COV genes and proteins are parsed from the GenBank files as features and assigned standard names based on their 
*product* tags. The synonyms for these standard names are listed in *cov_dictionary.yaml*.


# requirements
* Python3 and packages, including Biopython
* Aligner (muscle, or clustalo, or mafft)
* HMMER


# to-do
* Analyze alignment and remove sequences without similarity
* Trim alignments before creating HMMs
