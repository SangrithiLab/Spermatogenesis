### Single-Cell RNA Sequencing of the *Cynomolgus* Macaque Testis Reveals Conserved Transcriptional Profiles during Mammalian Spermatogenesis

### Graphical Abstract
<img src="./Images/GraphicalAbstract.png" width=500>

### Data availability and code
We utilized testis-specific scRNA-Seq data generated from three species (macaque, human, and mouse), and the raw data is publicly available.
  1. Our own macaque dataset - this study (ArrayExpress: [E-MTAB-8979](https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-8979/)).
  2. Human datasets - (i) Hermann et al., 2018 (GEO: [GSE109037](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE109037)) and (ii) Guo et al., 2018 (GEO: [GSE120508](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE120508)).
  3. Mouse dataset - Ernst et al., 2019 (ArrayExpress: [E-MTAB-6946](https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-6946/)).

The codes used to analyse all the datasets are provided as Jupyter Notebooks available under the [Analysis](../master/Analysis/) folder and the HTMLs of the notebooks are available under the [HTML](../master/HTML/) folder ([macaque](http://htmlpreview.github.io/?https://github.com/SangrithiLab/Spermatogenesis/blob/master/HTML/Macaque_scRNASeq_Analysis.html), [human](http://htmlpreview.github.io/?https://github.com/SangrithiLab/Spermatogenesis/blob/master/HTML/Human_scRNASeq_Analysis.html), and [mouse](http://htmlpreview.github.io/?https://github.com/SangrithiLab/Spermatogenesis/blob/master/HTML/Mouse_scRNASeq_Analysis.html)). 

To reproduce the analysis performed on the macaque dataset, follow the steps below to get started:
  #### 1. Retrieving data 
  ```shellscript
# Macaque cellranger matrix data
wget https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-8979/files/macaque_cellranger_matrix.mtx

# cells metadata
wget https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-8979/files/macaque_cells_metadata.txt

# genes metadata
wget https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-8979/files/macaque_genes_metadata.txt
```
  #### 2. Analysis
  Load the `Macaque_scRNASeq_Analysis-Reproduce.ipynb` file available under the [analysis](../master/Analysis/) folder and run the cells. <br>
  **Note: Make sure the .ipynb and the downloaded files are in the same folder.**
