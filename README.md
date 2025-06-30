# Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster
This repository houses all processed data files and the complete analytical codebase utilized for my biology dissertation. It supports the findings presented in "Atlas of the chromatin landscape in the developing nervous system of Drosophila melanogaster" by providing full reproducibility and access to the underlying computational work.

Supplementary Material
All processed data and analysis code for this dissertation have been made publicly accessible. In particular, a GitHub repository [(e.g. https://github.com/… as provided to reviewers)](https://github.com/Neura1net/Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster/edit/main/README.md) contains all scripts and processed datasets generated in this work. This repository replicates the original folder structure and includes the following content:

•	BiTS_ATAC_data_dm6_Glahs_Karabacak: Results of the BiTS ATAC-seq experiments (peak calls, DESeq2 results tables, multiBamCov inputs, and normalized signal files).

•	BiTS_ChIP_Differential_enrichment_analysis_at_TSS_and_Enhancers: Results of the BiTS ChIP-seq differential enrichment analysis (DESeq2 results, multiBamCov inputs, clustering outputs, and integrated RNA-seq tables). This folder also includes the master DRG and enhancer analysis tables. All pairwise comparisons are summarized in Supplementary Figure 1 of the thesis.

•	BiTS_ChIP_Normalised_Signal_files_dm6_Glahs: RPGC-normalized, background-subtracted ChIP-seq signal tracks for the BiTS ChIP experiments.

•	BiTS_ChIP_TAD_Analysis_Supplement_dm6_Glahs: Results of the Hi-C TAD analysis described in Chapter 8.8.

•	EpicSeg_HMM_dm6_Supplement_Glahs: Hidden Markov Model (HMM) parameters, segmentation results, and state-transition data for the epicSeg chromatin-state analysis.


Raw sequencing data (original FASTQ files for all ATAC-seq and ChIP-seq libraries) are archived on an external hard drive at the Humboldt-Universität Library. These raw data are available on request (for example, via the Library’s research data service desk) for any interested reader. This arrangement ensures long-term preservation and accessibility of the raw datasets, in line with institutional research-data policies.
