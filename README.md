
[![INSERT YOUR GRAPHIC HERE](https://personalpages.manchester.ac.uk/staff/jing.yang/Data/MRC_figure1.png)]()

# Simultaneous analysis of open chromatin, promoter interactions and gene expression in stimulated T cells implicates causal genes for rheumatoid arthritis
 scripts to accompany the paper [**"Simultaneous analysis of open chromatin, promoter interactions and gene expression in stimulated T cells implicates causal genes for rheumatoid arthritis"**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/manuscript.pdf) authored by <i>Jing Yang, Amanda McGovern,  Paul Martin, Kate Duffus, Peyman Zarrineh, Andrew P Morris, Antony Adamson, Peter Fraser, Magnus Rattray & Stephen Eyre</i>. Scripts are based on R and presented in Jupyter notebook. 

## Table of contents:
- [ATACseq](#ATACseq)
- [RNAseq](#RNAseq)
- [CHiC](#CHiC)
- [HiC](#HiC)
- [Linking_CHiC_ATACseq_RNAseq](#Linking_CHiC_ATACseq_RNAseq)

## ATACseq
- [**ATACseq_calculate_LRandBIC.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_calculate_LRandBIC.ipynb): calculate Loglikelihood ratio (LR) and bayesian information criteria (BIC) for ATAC-seq data.
- [**ATACseq_heatmap_Fig_3a.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_heatmap_Fig_3a.ipynb): heatmap of ATAC-seq data based on the clustering results from ATACseq_clustering_Fig_3c.ipynb.
- [**ATACseq_clustering_Fig_3c.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_clustering_Fig_3c.ipynb): hierarchical Gaussian Processing (GP) clustering of dynamic ATAC-seq time course data.
- [**ATACseq_correlation_Fig_3b.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_correlation_Fig_3b.ipynb): display the correlation between replicates of ATAC-seq peaks.
- [**ATACseq_supplementary_Fig_3a.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_supplementary_Fig_3a.ipynb): histogram of the ATAC-seq peak size distribution.
- [**ATACseq_supplementary_Fig_3b.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_supplementary_Fig_3b.ipynb): piechart plot of annotation of ATAC-seq peaks.

## RNAseq
- [**RNAseq_correlation_exon_intron_check.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/RNAseq/RNAseq_correlation_exon_intron_check.ipynb): illustrate the correlations between exons and introns counts data from RNA-seq samples. Figures are shown in Supplementary Fig. 2a-c. 
- [**RNAseq_correlation_histogram.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/RNAseq/RNAseq_correlation_histogram.ipynb): display the histogram of correlation coefficients between RNA-seq replicated data. Figure is shown in Supplementary Fig. 2d
- [**RNAseq_quality_check_withdatafromYe.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/RNAseq/RNAseq_quality_check_withdatafromYe.ipynb): compare the gene expression data from this study with the data from **"Ye, C. J., et al. "Intersection of population variation and autoimmunity genetics in human T cell activation." Science 345.6202 (2014): 1254665"**.

## CHiC
- [**CHiC_qualitycheck.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/CHiC/CHiC_qualitycheck.ipynb): compare CHi-C interactions with similar data from **"Burren, O.S. et al, Chromosome contacts in activated T cells identify autoimmune disease candidate genes, Genome Biology, 18 (165) (2017)"** 
- [**CHiC_clustering.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/CHiC/CHiC_clustering.ipynb): clustering of CHi-C data and generate Supplementary Fig. 1b

## HiC
- [**HiC_interaction_matrices.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/HiC/HiC_interaction_matrices.ipynb): generate the interaction matrices for Hi-C data at different time. Upper triangular part of Hi-C data of chr1 is shown in Fig. 2a
- [**HiC_correlations_plot.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/HiC/HiC_correlations_plot.ipynb): compute the Stratum adjusted Correlation Coefficient (SCC) between Hi-C datasets and generate Fig. 2b.
- [**ABcompartment_correlations_plot.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/HiC/ABcompartment_correlations_plot.ipynb): compute the correlation coefficients of A/B compartment data and display Fig. 2c. 
- [**ABcompartment_SNPs_overlap.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/HiC/ABcompartment_SNPs_overlap.ipynb): illustrate the overlap of rheumatoid arthritis SNPs and A/B compartments at different times.      

## Linking_CHiC_ATACseq_RNAseq
Directory for producing correlation density plots between linked CHi-C, ATAC-seq and RNA-seq data.
- [**plot_CHiC_ATACseq_RNAseq_connections_Fig4a.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_CHiC_ATACseq_RNAseq_connections_Fig4a.ipynb): generate the correlation density maps of linked CHi-C, ATAC-seq and RNA-seq data under varied distance ranges around promoters.
- [**plot_foldchange_Fig4bc.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_foldchange_Fig4bc.ipynb): display the log2 fold change of ATAC-seq vs gene and CHi-C vs gene, as shown in Fig. 4b-c
- [**plot_supplementary_Fig_5.ipynb**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_supplementary_Fig_5.ipynb): display dynamic patterns of CHi-C and ATAC-seq associated with different gene clusters. 

For more clarification, please feel free to contact Jing Yang via : Jing.Yang@manchester.ac.uk
