# MCF10A-Bulk-RNA-Sequencing
 Analysis of metabolic perterbations of MCF10A cells


Analysis of MCF10A cells in 16 different conditions 2 biological replicates
per sample. Note that we would ideally need at least three replicates for a standard analysis.

After running STAR alignment, one of the outputs will be the raw counts per gene in each sample. 
We will use DESeq2 to detect differentially expressed genes. 

A key aspect of analysis involves quantifying and statistically inferring systematic changes between conditions, contrasting them with within-condition variability. DESeq2, a software package, employs negative binomial generalized linear models to assess differential expression. The estimates of dispersion and logarithmic fold changes integrate data-driven prior distributions.

More information about the DESeq workflow can be found at: https://bioconductor.org/packages/devel/bioc/vignettes/DESeq2/inst/doc/DESeq2.html
Love, M.I., Huber, W., Anders, S. (2014) Moderated estimation of fold change and dispersion for RNA-seq data with DESeq2. Genome Biology, 15:550. 10.1186/s13059-014-0550-8
