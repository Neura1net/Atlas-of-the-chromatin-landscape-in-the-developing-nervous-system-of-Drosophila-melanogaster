# Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster
This repository houses all processed data files and the complete analytical codebase utilized for my biology dissertation. It supports the findings presented in "Atlas of the chromatin landscape in the developing nervous system of Drosophila melanogaster" by providing full reproducibility and access to the underlying computational work.


**DOI of the original Disseration with the Title "Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster":** DOI:XXXX.XXXX

**DOI of this collection of suplemental data:** DOI:XXXX.XXXX

**Supplementary Material**
All processed data and analysis code for this dissertation have been made publicly accessible. In particular, a GitHub repository [(Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster/edit/main/README.md)](https://github.com/Neura1net/Atlas-of-the-chromatin-landscape-in-the-developing-nervous-system-of-Drosophila-melanogaster/edit/main/README.md) contains all scripts and processed datasets generated in this work. This repository replicates the original folder structure and includes the following content:

•	BiTS_ATAC_data_dm6_Glahs_Karabacak: Results of the BiTS ATAC-seq experiments (peak calls, DESeq2 results tables, multiBamCov inputs, and normalized signal files).

•	BiTS_ChIP_Differential_enrichment_analysis_at_TSS_and_Enhancers: Results of the BiTS ChIP-seq differential enrichment analysis (DESeq2 results, multiBamCov inputs, clustering outputs, and integrated RNA-seq tables). This folder also includes the master DRG and enhancer analysis tables. All pairwise comparisons are summarized in Supplementary Figure 1 of the thesis.

•	BiTS_ChIP_Normalised_Signal_files_dm6_Glahs: RPGC-normalized, background-subtracted ChIP-seq signal tracks for the BiTS ChIP experiments.

•	BiTS_ChIP_TAD_Analysis_Supplement_dm6_Glahs: Results of the Hi-C TAD analysis described in Chapter 8.8.

•	EpicSeg_HMM_dm6_Supplement_Glahs: Hidden Markov Model (HMM) parameters, segmentation results, and state-transition data for the epicSeg chromatin-state analysis.

Raw sequencing data (original FASTQ files for all ATAC-seq and ChIP-seq libraries) will be archived on the EDOC-Server at the Humboldt-Universität Library (DOI:XXXXX.XXXX). These raw data are available via the HU Berlin Library’s research data service (EDOC) for any interested reader. This arrangement ensures long-term preservation and accessibility of the raw datasets, in line with institutional research-data policies.

**DDC classification:** 574.3 Developmental Biology

**Keywords:** 

Drosophila melanogaster

Central nervous system development

Neurogenic tissue specification

Neuroblast differentiation

Neuroectoderm (ventral column, intermediate column)

Stem cells

Genomic regulatory state

Histone modifications

Chromatin accessibility

Cis-regulatory modules (CRMs)

Differentially regulated genes (DRGs)

Spatiotemporal gene regulation

Differential peak calling

Differential enrichment analysis

Machine learning

Gene regulatory networks

Sequence motif enrichment

Tissue-specific gene regulation

Neurogenesis

Tissue differentiation


**Author:** Alexander Glahs

**Email:** aglahs@yahoo.de

**License:**
Atlas of the chromatin landscape in the developing nervous system of Drosophila
melanogaster © 2022 by Alexander Glahs is licensed under Creative Commons
Attribution-NonCommercial-ShareAlike 4.0 International. To view a copy of this license,
visit https://creativecommons.org/licenses/by-nc-sa/4.0/


**List of Abbreviations and Acronyms**

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

ATAC-seq Assay for Transposase- Accessible Chromatin using sequencing LSc Lethal of Scute

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

MEME Multiple Expectation maximizations for Motif Elicitation BMP bone morphogenetic protein miRNA microRNA
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

CRM Cis-regulatory module NetA/NetB Netrin-A / Netrin-B

CRN cis-regulatory network NFR nucleosome-free region

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
