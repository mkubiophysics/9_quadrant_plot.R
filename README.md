# 9_quadrant_plot.R
 R script to generate 9 quadrant plot for integrating transcriptomics and proteomics data

# Introduction
It is a single script to generate 9 quadrant plot that integarte RNAseq and LC-MS data and further generate quadrants with the genes/proteins commonly expressed in both datasets. 

# Pre-requiste
. R 

. R studio

. plotly

. ggplot2

# Installation
To install the 9_quadrant_plot.R script:

First clone the repository into a local directory:

```
git clone https://github.com/mkubiophysics/9_quadrant_plot.R.git
$ cd 9_quadrant_plot.R
```
# Prepare Input files

Generate a combined file with name `combined_data.csv` in the below described manner:

 ![image](https://github.com/user-attachments/assets/672112c7-49d4-4733-b7da-c3dd31c05e15)
 
Here, X stands for Log2FC values of proteins from proteomics data and Y stands for Log2FC values of genes from transcriptomics data [Detailed in Supplementary 3 of paper]

# Running the script

In R studio 

```
9_quadrant_plot.R
```
It will generate the plot.

Also, to get genes/proteins commonly expressed and present in 9 different quadarant. open the script and modify the directory name where the output will generate

For, example 

write.csv(quadrant_1, "$PATH/TO/YOUR/DIRECTORY" )

# Output Files

. 9 quadrant plot.png/pdf

. `quadrant_1.csv` `quadrant_2.csv` `quadrant_3.csv` `quadrant_4.csv` `quadrant_5.csv` `quadrant_6.csv` `quadrant_7.csv` `quadrant_8.csv` `quadrant_9.csv` consists of genes/proteins commonly expressed in both the datasets.

# Developer info

Manisha Aswal (maswal@biophysics.du.ac.in)


