# 9_quadrant_plot.R
 An R script to make 9 quadrant plot to integrate transcriptomics and proteomics expression data

# Introduction
It is a R script to make 9 quadrant plot that integarte RNAseq and LC-MS expression data. The objective of 9 quadrant plot is to separate genes that shows concordance and discordance in the expression at mRNA and protein levels. 
![Untitled (30)](https://github.com/user-attachments/assets/a31bda4d-9f7d-4775-9520-303249361662)


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

Also, to get genes/proteins commonly expressed and present in 9 different quadarant. open the script and modify the directory name where the output files will be saved

For, example 

write.csv(quadrant_1, "$PATH/TO/YOUR/DIRECTORY" )

# Output Files

. 9 quadrant plot.png/pdf

. `quadrant_1.csv` `quadrant_2.csv` `quadrant_3.csv` `quadrant_4.csv` `quadrant_5.csv` `quadrant_6.csv` `quadrant_7.csv` `quadrant_8.csv` `quadrant_9.csv` consists of genes/proteins commonly expressed in both the datasets.

# Developer info

Manisha Aswal (maswal@biophysics.du.ac.in)


