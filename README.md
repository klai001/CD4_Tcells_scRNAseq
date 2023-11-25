This is a re-analysis of single cell RNAseq of CSF cells. from the following GEO repo: GSE135477 https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE134577 The following are the key steps: preprocessing and QC of each sample type (e.g. HC,  AD) independently. normalization is via SCT integration is rPCA with annotated HC datasets as reference T cells (CD3+) positive cells are subset from the dataset, and then further subset into single positive CD4cells.RData or CD8cells.RData. Pseudotime trajectory using slingshot is performed on CD4cells. These trajectories were then used to extract differentially expressed genes across the lineage using tradeseq `associationTest()` function.
the smoothers were then plotted as a heatmap for comparison. 
Differential abundance was performed using MiloR- however, the condition effect was pretty weak (uniform pvalue histogram). 

PLEASE USE NBVIEWER TO VIEW THE SCRIPTS
