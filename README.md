# README


Readme for Acute Myeloid Leukemia Heatmap
Author: CCDL for ALSF - Adapted for this repository by Candace Savonen
Modified by: Martiela Freitas
Date: October 2021

Last Updated: October 2021

Goals:

This script analyses RNA-seq data from a study on Acute Myeloid Leukemia (AML)
The script creates a clustered heatmap to identify groups of genes with similar expression patterns across different samples.
The heatmap is further annotated with treatment information for each sample.
Software needed:

R version needs to be compatible with the included packages
Required Packages:
pheatmap (for heatmap generation and clustering)
dplyr (for data manipulation)
magrittr (for piping functionality)
readr (for reading tsv files)
tibble (for data manipulation)
sessioninfo (for printing session information)
File Locations:

The script assumes the data is downloaded from refine.bio and placed in a folder named "data" within the project directory.
The script creates folders named "plots" and "results" to store generated plots and intermediate files respectively.
How to Run:

Download the data from refine.bio following the link in the script (https://www.refine.bio/experiments/SRP070849).
Place the downloaded data folder named "SRP070849" within a folder named "data" in your project directory.
Open the script in an R environment and run the entire script.
The script will generate a heatmap named "aml_heatmap.png" within the "plots" folder.
Additional Notes:

This script is adapted from a publicly available example from refine.bio (https://alexslemonade.github.io/refinebio-examples/03-rnaseq/clustering_rnaseq_01_heatmap.html).
The heatmap displays the top 25% of genes with the highest variance across samples.
The script colors the heatmap based on the gene expression with blue representing low expression and yellow representing high expression.
The heatmap is further annotated with treatment information for each sample.