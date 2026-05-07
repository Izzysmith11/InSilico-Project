Code for analysis of OneK1K dataset to identify MS-associated genes.
1. QC
   Removed cells with percentage of mitochondrial genes greater than or equal to 20%
   Scale factor of 10,000 was used for normalisation
   Top 2000 variable genes were selected and used to scale the data
   Dimensionality reduction was performed using PCA
   Clusters and marker genes were identified
   Sanity checks were performed
2. Subset pbmc3k data into different cell types
   B cells
   CD4 T cells
   CD8 T cells
   Monocytes
   NK cells
3. Differential gene expression performed on each cell type comparing:
   Males vs females
   Young vs old females
   Young vs old males
4. DGE results filtered with list of MS-associated genes from GWAS
5. UMAPs were created to show cell types and expression of most significant MS-genes from DGE
