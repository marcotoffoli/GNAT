# GNAT

#GNAT (GBA Nanopore Analysis Tool) si a wrapping script for analysing PCR targeted sequencing of the GBA gene, as reported in https://www.medrxiv.org/content/10.1101/2021.11.12.21266253v1.full

#To make it work, all dependencies installed and added to PATH (NGMLR, bgzip, tabiz, annovar, whatshap, vcftools, bcftools, Clair).

#usage: GNAT -q /path/to/folder_with_fastq  -w /path/to/folder_for_output -r /path/to/reference_for_alignment -b /path/to/bed_file_with_full_GBA_coverage -Q threshold_for_QG_filtering_of_called_variants -t target_region(format chrx:nnnnnnnnn-nnnnnnnnn)[default chr1:155234452-155241249] -C /path/to/clair.py -cm /path/to/clair/modules/folder

#I installed Clair without conda environments so that it works by just calling python /path/to/clair.py. If you installed it differently you will have to update the script to activate and deactivate environments

#please see our publication for more information. 

#Please reference our paper if using the script https://www.medrxiv.org/content/10.1101/2021.11.12.21266253v1
