README —
Atlas of the Chromatin Landscape in the Developing Nervous System of Drosophila melanogaster
Alexander Glahs (Doctoral dissertation, 2022)

GitHub repository: https://github.com/Neura1net/Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster. (GitHub)
This repository houses all processed data files and the complete analytical codebase utilized for my biology dissertation. It supports the findings presented in "Atlas of the chromatin landscape in the developing nervous system of Drosophila melanogaster" by providing full reproducibility and access to the underlying computational work.


________________________________________
Table of contents
1.	Purpose & scope
2.	Persistent identifiers
3.	Data availability & archiving
4.	Repository contents (exact folder names)
5.	File types & conventions
6.	Provenance & methods
7.	Reproducibility notes
8.	How to cite
9.	License
10.	Author, classification & contact
11.	Keywords
12.	Abstract (concise publication form)
13.	List of abbreviations and acronyms
14.	Acknowledgements
________________________________________
Purpose & scope
This repository contains the processed data files and the complete analysis codebase produced for the doctoral dissertation:
Atlas of the chromatin landscape in the developing nervous system of Drosophila melanogaster (A. Glahs, 2022).
Materials provided here enable reproduction of the computational results, figures and tables presented in the dissertation and provide a comprehensive resource for comparative and follow-up studies of chromatin regulation during neurogenesis.
________________________________________
Persistent identifiers
•	Dissertation DOI: DOI:XXXX.XXXX
•	DOI for this supplemental data collection: DOI:XXXX.XXXX
________________________________________
Data availability & archiving
•	Processed data and analysis code are hosted in this GitHub repository. (GitHub)
•	Raw sequencing data (FASTQ files) will be archived at the Humboldt-Universität zu Berlin EDOC server and made available via the HU Library research-data service (EDOC). The EDOC archive will provide long-term preservation and institutional access in accordance with HU data-management policies.
________________________________________
Repository contents 
This repository reproduces the original folder layout used during the dissertation work. The top-level folders are listed below exactly as they appear in the repository:

•	BiTS_ATAC_data_dm6_Glahs_Karabacak/
Results of the BiTS ATAC-seq experiments: peak calls, DESeq2 differential accessibility tables, multiBamCov input/count files and normalized signal tracks (dm6).

•	BiTS_ChIP_Differential_enrichment_analysis_at_TSS_and_Enhancers/
BiTS ChIP-seq differential enrichment results: DESeq2 outputs, multiBamCov inputs, clustering analyses, RNA-seq integration tables, and the master DRG and enhancer analysis tables. All pairwise comparisons referenced in the dissertation are summarized in Supplementary Figure 1 of the dissertation.

•	BiTS_ChIP_Normalised_Signal_files_dm6_Glahs/
RPGC-normalized and background-subtracted ChIP-seq signal tracks (bigWig / bedGraph) produced for visualization and quantitative analyses.

•	BiTS_ChIP_TAD_Analysis_Supplement_dm6_Glahs/
Hi-C / TAD analysis results (domain coordinates, boundary strength metrics and associated supplementary tables/figures) discussed in Chapter 8.8 of the dissertation.

•	EpicSeg_HMM_dm6_Supplement_Glahs/
EpicSeg (HMM) model parameters, segmentation outputs (state BEDs), emission/transition parameter tables and state-transition diagnostics.

•	Software und Code Repository - R - Analysis/
Primary R analysis scripts and helper functions used to generate tables, statistical analyses and figures. This folder documents the analysis pipeline and references per-analysis metadata where available.

•	README.md (this file).
________________________________________
File types & conventions
Files in this repository follow standard genomics and data-science conventions:

•	BED — genomic intervals (peaks, TADs, segmentation states). Coordinates are relative to dm6 (D. melanogaster) unless stated otherwise.

•	bigWig / bedGraph — continuous normalized signal tracks for genome-browser visualization.

•	TSV / CSV — tabular differential results (DESeq2), master tables, summary statistics, integration tables.

•	PDF / PNG — high-resolution figures and diagnostic plots used in the dissertation.

•	R scripts — analysis code (located in Software und Code Repository - R - Analysis/); scripts include inline documentation and references to package requirements where applicable.
________________________________________
Provenance & methods

•	All processed files are mapped to the D. melanogaster dm6 reference assembly. Users should confirm genome-build consistency before integrating these data with external resources.

•	Detailed descriptions of data preprocessing, normalization choices, statistical models (DESeq2 settings, multiple-test adjustments), segmentation parameters, and clustering criteria are provided in the dissertation Methods section.
________________________________________
Reproducibility notes

•	The Software und Code Repository - R - Analysis/ folder contains the R scripts used to reproduce the major tables and figures. Scripts reference the primary inputs and indicate required packages.

•	Exact software versions, parameter choices and preprocessing steps are described in the Methods section of the dissertation; reviewers and users attempting byte-for-byte reproduction should consult those sections and the per-folder metadata.
________________________________________
How to cite

When using these data, code or figures please cite both the dissertation and this repository:

Dissertation (primary citation):

Glahs, A. (2022). Atlas of the chromatin landscape in the developing nervous system of Drosophila melanogaster. Doctoral dissertation, Humboldt-Universität zu Berlin. DOI: DOI:XXXX.XXXX.

Supplemental collection (this repository):

Glahs, A. (2022). Supplemental data and analysis code for “Atlas of the chromatin landscape in the developing nervous system of Drosophila melanogaster.” GitHub repository, Neura1net. https://github.com/Neura1net/Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster. (GitHub)
________________________________________
License

© 2022 Alexander Glahs.

This work is licensed under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0). To view the full license terms see: https://creativecommons.org/licenses/by-nc-sa/4.0/.
________________________________________
Author, classification & contact

•	Author: Alexander Glahs

•	Email: aglahs@yahoo.de

•	DDC classification: 574.3 — Developmental Biology

For questions regarding data provenance, metadata, or access to the raw sequencing files archived in EDOC, please contact the author.
________________________________________
Keywords

Drosophila melanogaster; central nervous system development; neurogenic tissue specification; neuroblast differentiation; neuroectoderm; stem cells; genomic regulatory state; histone modifications; chromatin accessibility; cis-regulatory modules (CRMs); differentially regulated genes (DRGs); spatiotemporal gene regulation; differential peak calling; differential enrichment analysis; machine learning; gene regulatory networks; motif enrichment; tissue-specific regulation; neurogenesis; tissue differentiation.
________________________________________
Abstract

In this study, I identify novel regulatory nodes and potential signal transduction pathways that govern neurogenic tissue specification and differentiation. The Drosophila melanogaster central nervous system develops from three columns of neuroectodermal cells that give rise to neural stem cells called neuroblasts. I investigated the genomic regulatory state of cells derived from the ventral column (VC) and the intermediate column (IC) of the neurectoderm (NE) as they specify, diversify and differentiate. In this thesis I investigated how cell populations become distinct from one another, and how the genomic regulatory state within these cell populations changes over developmental time. As post-translational histone modification occupancy and chromatin accessibility has been linked to distinct aspects of gene regulation, I assessed their tissue specific genome wide distributions and used them as a proxy to investigate the genomic regulatory state in a developing embryo. Differential peak calling, differential enrichment analysis and machine learning was employed to identify spatiotemporally regulated cis- regulatory modules (CRMs) and differentially regulated genes (DRGs). I could show that I can accurately predict tissue specific CRMs by validating a subset of de novo predicted differentially regulated CRMs with reporter lines. The spatiotemporal regulatory trajectory of differentially regulated elements was used to refine the existing models for the gene regulatory networks that govern neuronal differentiation, to associate distal regulatory elements with core promoters, and to identify enriched sequence motifs within active CRMs. Taken together the datasets and algorithms in this study provide a comprehensive atlas of novel CRMs of the developing nervous system in Drosophila, novel insights into the regulatory nodes and edges during neurogenesis and a valuable resource to refine existing models of neurogenesis specifically and tissue differentiation generally.
________________________________________
Acknowledgements

The data, analyses and curation presented in this repository were produced as part of the doctoral research conducted at Humboldt-Universität zu Berlin. Raw sequencing data will be archived in the EMBL/EBI ArrayExpress Repository to guarantee long-term preservation and institutional access. (https://www.ebi.ac.uk/biostudies/arrayexpress)

________________________________________
List of abbreviations and acronyms


**List of Abbreviations and Acronyms:**

3’UTR 3′ untranslated region 

K27ac H3K27ac

3D Three-dimensional 

K27me3 H3K27me3

5’UTR 5′ untranslated region 

K4me1 H3K4me1

A/P anterior–posterior axis 

K4me3 H3K4me3

AA amino acid 

K79me3 H3K79me3

AB antibody 

kb kilobase

ab abrupt 

KCl Potassium chloride

AED after egg deposition 

kni knirps

AEL after egg laying 

Kr Kruppel

AMG anterior midgut 

LAD Lamina-associated domains

Antp Antennapedia 

LC lateral collumn

aop anterior open /yan 

LCR Locus control regions
aos argos 

LIM LIN-11, Isl1 and MEC-3

AP alcaline phosphatase 

LLPS liquid-liquid phase separation 

aPKC atypical protein kinase C 

lncRNA Long non-coding RNA

AR androgen receptor 

Loco Locomotion defects

AS amnioserosa 

LOF Loss-of-Function

AS-C achaete-scute complex 

log2FC log2 fold change

ATAC-seq Assay for Transposase- Accessible Chromatin using sequencing 

LSc Lethal of Scute

Awh Arrowhead 

LSFM Light sheet fluorescence microscopy

Bap Bagpipe 

mAB monoclonal antibody

BCIP 5-Bromo-4-chloro-3-indolyl phosphate 

MAPK mitogen-activated protein-kinase

BDGP Berkeley Drosophila Genome Project 

MCS multiple cloning site

bHLH Basic helix–loop–helix mef2 myocyte enhancer factor-2

BiTS-ChIP batch isolation of tissue-specific chromatin for immunoprecipitation

MEME Multiple Expectation maximizations for Motif Elicitation 

BMP bone morphogenetic protein 

miRNA microRNA

bp base pair 

mirr mirror

BSA bovine serum albumin 

MNase Micrococcal nuclease

cas castor 

mod(mdg4) modifier of mdg4

CBP CREB-binding protein 

MS/MS tandem mass spectrometry

chinmo chronologically inappropriate morphogenesis 

msh muscle segment homeobox / Drop

ChIP chromatin immunoprecipitation 

μl microliter 

cic capicua 

μm micrometre

CLSM Confocal laser scanning microscopy 

N Notch

CNS central nervous system 

NaCl Sodium chloride

CoIP co-immunoprecipitation 

NB neuroblasts

CRE Cis-regulatory element 

NBT Nitro blue tetrazolium chloride

CREB cAMP response element-binding protein 

nc negative control

CREM cAMP response element

modulator NE neurectoderm

CRM Cis-regulatory module

NEE neuroectodermal enhancer

CRM Cis-regulatory module 

NetA/NetB Netrin-A / Netrin-B

CRN cis-regulatory network 

NFR nucleosome-free region

ct cut 

Ni-NTA Nickel-nitrilotriacetic acid

CTCF CCCTC-binding factor 

NMD nonsense-mediated decay

cv crossveinless 

nub nubbin

D Dicheate 

oc ocelliless

D.mel Drosophila melanogaster 

odd odd skipped

D/V dorso-ventral axis 

ORF open reading frame

DAPI 4′,6-diamidino-2-phenylindole 

os/upd1 outstretched / unpaired 1

Dfd Deformed 

PBS phosphate buffered saline

DIG digoxigenin 

PCC Pearson correlation coefficient

DNA deoxyribonucleic acid 

PCR Polymerase chain
reaction

DNAse deoxyribonuclease 

PET Prickle Espinas Testin

doc1-3 dorsocross 1-3 

PHM pharingeal musculature

dpERK phosphorylated form of
MAPK/Erk 

Pins Partner of Inscuteable

dpp decapentaplegic 

piRNA Piwi-interacting RNA

DRE differentially-regulated
element 

Plc21C Phospholipase C at 21C

DREME Discriminative Regular
Expression Motif Elicitation 

pMad Phosphorylated Mothers
against decapentaplegic

DRG differentially-regulated
genes 

PMG posterior midgut

E(spl) Enhancer-of-split 

PMG posterior midgut

ECM extracellular matrix 

pnr pannier

EDTA Ethylenediaminetetraacetic
acid 

PNS peripheral nervous
system

eGFP enhanced Green
fluorescent protein 

pnt pointed

EGFR Epidermal growth factor
receptor PolII RNA polymerase II

EGTA ethylene glycol-bis(β-
aminoethyl ether)-N,N,N′,N′-
tetraacetic acid)

Pon Partner of Numb

EL early/late 

prd paired
ems empty spiracles 

PTM prothoracic mesoderm
en engrailed 

PTM post-translational
modification

Enh. Enhancer 

EpiCSeg Epigenome Count-based
Segmentation 

qRT-PCR
Real-Time Quantitative
Reverse Transcription
PCR

ERK extracellular signal-
regulated kinases 

RBP RNA binding protein

esn Espinas 

RefSeq NCBI Reference
Sequences

ETS E26 transformation specific 

RFP Red fluorescent protein
eve even skipped 

rho rhomboid

ey eyeless 

RNA Ribonucleic acid

eya eyes absent 

RNA-Seq RNA sequencing

eyg Eyegone 

RPGC reads per genomic
content

FACS fluorescence-activated
single cell sorting scATAC single cell ATAC

FISH Fluorescence in situ
hybridization 

scChIP single cell ChIP

FITC Fluorescein isothiocyanate 

SDS-PAGE
sodium dodecyl sulfate
polyacrylamide gel
electrophoresis

fkh fork h

ead shep alan shepard
FMP fused midgut primordium 

shn schnurri

FOXO1 fork head box protein O1 

sim singleminded
FT flowthrough 

siRNA Small interfering RNA
ftz fushi tarazu 

SM somatic musculature

g standard acceleration due
to gravity 

sog short gastrulation

G1/G0
entry of a quiescent cell
back into the cell cycle
stage G1

SoxN SoxNeuro

G1/S boundary between the G1
phase and the S phase SRF Serum response factor

GAM Genome Architecture
Mapping St. Stage

GFP Green fluorescent protein 

STARR
self-transcribing active
regulatory region
sequencing

GMC ganglion mother cell 

Su(var)3-9 Suppressor of
variegation 3-9

GMO genetically modified
organism 

Svp seven up
GO Gene Ontology 

T1-3 thoracic segments 1-3
GOF Gain-of-Function 

TAD topologically associated
domains

GP Glial Precursor 

TES Transcription End Site
Gt Giant 

Tet
Ten-Eleven
Translocation family
protein

h hairy 

TET Ten-Eleven
Translocation

h hours 

TF Transcription factor

H3 Histone H3 

TFBS transcription factor
binding site

HAT Histone acetyltransferases
 
Tin Tinman

Hb Hunchback 

tkv thickveins

hbs hibris 

Tl Toll

HDAC Histone deacetylases 

toe twin of eyegone

HG hindgut 

TSA Tyramide Signal
Amplification

hh hedgehog 

tsh teashirt

HIPK2 Homeodomain-interacting

protein kinase 2 

Tsp Thrombospondin

HLH helix–loop–helix 

TSS Transcription start sites
HMG High-Mobility Group 

TTS Transcription termination
sites

HMM Hidden Markov model 

twi twist

hnt hindsight 

UAS upstream activator
sequence

HP1 Heterochromatin protein 1 

ush u-shaped

HRP horseradish peroxidase 

vas vasa

hth homothorax 

VC ventral collumn

IC intermediate collumn 

vn vein

ICR Imprinting control region VNC ventral nerve cord

IDR irreproducible recovery rate vnd ventral nervous system
defective

IFA indirect
immunofluorescence assay VT Vienna Tile

ind intermediate neuroblasts
defective 

w white
Inv Invected 

wg wingless

IP input 

WNK with no lysine (K) protein
kinases

IPTG isopropyl β-D-1-
thiogalactopyranoside 

wor worniu

ISH In situ hybridization 

y yellow

JAK/STAT Janus kinase-signal
transducer and activator of
transcription

yan anterior open /yan

JNK c-Jun N-terminal kinases 

zen zerknüllt
