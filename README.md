
[![INSERT YOUR GRAPHIC HERE](https://personalpages.manchester.ac.uk/staff/jing.yang/Data/MRC_figure1.png)]()

# Analysis of chromatin organization and gene expression in T cells identifis functional genes for rheumatoid arthritis
 scripts to accompany the paper [**"Analysis of chromatin organization and gene expression in T cells identifies functional genes for rheumatoid arthritis"**](https://github.com/ManchesterBioinference/Publications/blob/master/IntegratingATAC-RNA-HiC/manuscript.pdf) authored by <i>Jing Yang, Amanda McGovern,  Paul Martin, Kate Duffus, Xiangyu Ge, Peyman Zarrineh, Andrew P Morris, Antony Adamson, Peter Fraser, Magnus Rattray & Stephen Eyre</i>. Scripts are based on R and presented in Jupyter notebook. 

## Table of contents:
- [ATACseq](#ATACseq)
- [RNAseq](#RNAseq)
- [CHiC](#CHiC)
- [HiC](#HiC)
- [Linking_CHiC_ATACseq_RNAseq](#Linking_CHiC_ATACseq_RNAseq)

## ATACseq
- [**Heatmap**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_heatmap_Fig_3a.ipynb): heatmap of ATAC-seq data based on the clustering results from ATACseq_clustering_Fig_3c.ipynb.
- [**Clustering**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_clustering_Fig_3b.ipynb): hierarchical Gaussian Processing (GP) clustering of dynamic ATAC-seq time course data.
- [**QC**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_supplementary_Fig_3.ipynb): quality check of ATAC-seq data.
- [**Dynamics**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/ATACseq/ATACseq_calculate_LRandBIC.ipynb): calculate Loglikelihood ratio (LR) and bayesian information criteria (BIC) for ATAC-seq data.

## RNAseq
- [**Correlation between exons and introns**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/RNAseq/RNAseq_correlation_exon_intron_check_supplementary_Fig1a-c.ipynb): illustrate the correlations between exons and introns counts data from RNA-seq samples. Figures are shown in Supplementary Fig. 1a-c. 
- [**PCA**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/RNAseq/RNAseq_supplementary_Fig1d.ipynb): display PCA results of RNA-seq data. Figure is shown in Supplementary Fig. 1d
- [**QC**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/RNAseq/RNAseq_quality_check_withdatafromYe_supplementary_Fig1e-i.ipynb): compare the gene expression data from this study with the data from **"Ye, C. J., et al. "Intersection of population variation and autoimmunity genetics in human T cell activation." Science 345.6202 (2014): 1254665"**. Figures are shown in Supplementary Fig. 1e-i

## CHiC
- [**QC**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/CHiC/CHiC_qualitycheck_supplementaryFig6a.ipynb): compare CHi-C interactions with similar data from **"Burren, O.S. et al, Chromosome contacts in activated T cells identify autoimmune disease candidate genes, Genome Biology, 18 (165) (2017)"** as shown in Supplementary Fig. 6a. 
- [**Clustering**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/CHiC/CHiC_clustering_supplemtnaryFig6b.ipynb): clustering of CHi-C data and generate Supplementary Fig. 6b.

## HiC
- [**Interactions**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/HiC/HiC_interaction_matrices.ipynb): generate the interaction matrices for Hi-C data at different time. Upper triangular part of Hi-C data of chr1 is shown in upper panel of Fig. 2a
- [**QC**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/HiC/Fig_2b_2c_HiC_ABcompartment_correlations_plot.ipynb): compute the Stratum adjusted Correlation Coefficient (SCC) between Hi-C datasets (Fig. 2b) and A/B compartments (Fig. 2c), respectively.
- [**SNPs**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/HiC/ABcompartment_SNPs_overlap.ipynb): illustrate the overlap of rheumatoid arthritis SNPs and A/B compartments at different times as shown in the lower panel of Fig. 2a.    
- [**Dynamics**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/HiC/TADs_percentage_plot_Supplementary_Fig7.ipynb): illustrate the percentage changes of TADs, compartment As and compartment Bs over time as illustrated in Supplementary Fig. 7 

## Linking_CHiC_ATACseq_RNAseq
Directory for producing correlation density plots between linked CHi-C, ATAC-seq and RNA-seq data.
- [**Correlations**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_CHiC_ATACseq_RNAseq_connections_Fig4a.ipynb): generate the correlation density maps of linked CHi-C, ATAC-seq and RNA-seq data under varied distance ranges around promoters as shown in Fig. 4a.
- **Dynamics**: dynamics of CHi-C, ATAC-seq, RNA-seq at different levels. 
  -  [**Dynamics in foldchange**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_foldchange_Fig4bc.ipynb): display the log2 fold change of ATAC-seq vs gene and CHi-C vs gene, as shown in Fig. 4b-c
  -  [**Dynamics in original data**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_supplementary_Fig_11.ipynb): display dynamic patterns of CHi-C and ATAC-seq associated with different gene clusters. 
  -  [**Dynamics at CTCF/H3K27AC binding sites**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_supplementary_Fig_10_a_b_c.ipynb): display dynamics of CHi-C, ATAC-seq and Gene expression linked to ATAC-seq peaks intersected with CTCF/H3K27AC binding sites.
  -  [**Dynamics at transcription factor binding sites**](https://github.com/ManchesterBioinference/blob/master/IntegratingATAC-RNA-HiC/Linking_CHiC_ATACseq_RNAseq/plot_supplementary_Fig_10d.ipynb): display dynamics of CHi-C at ATAC-seq peaks intersected with CTCF/H3K27AC/NFKB binding sites.

For more clarification, please feel free to contact Jing Yang via : Jing.Yang@manchester.ac.uk
