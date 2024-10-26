# **Revealing gene-level variations in Arabidopsis**

## **Introduction**
 
The analysis of genomic rearrangements between closely related species and ecotypes provides insights into evolutionary changes that may have contributed to adaptation to different environmental conditions. In this study, we analysed gene-level rearrangements between the *Arabidopsis thaliana* TAIR10.1 reference assembly (GCF_000001735.4), the *Cdm-0* ecotype (GCA_904420315.1) and another species of the Arabidopsis genus, *A.arenosa* (GCA_905216605.1). Comparison of these three genomes at the gene level aims to identify potentially significant structural rearrangements that may have arisen during evolution.

To accomplish this task, tools for visualisation and analysis of genomic rearrangements were used, such as mummerplot to plot comparative plots between genomes and MCScan to plot synteny. These methods allowed us to identify structural differences in the gene arrangement of these Arabidopsis ecotypes and species.
 
## **Methods**

Files in .fasta and .gff formats for TAIR10.1, Cdm-0 and A. arenosa assemblies were downloaded for analysis. Data for TAIR10.1, Cdm-0, and A. arenosa assemblies were obtained from NCBI databases and contained complete genome sequences and annotations for each sample. Conversion of GFF files to BED format, as well as isolation of coding regions (CDS) required for further work, was performed using the AGAT package.

The mummerplot tool was used to identify and visualise genomic rearrangements between genomes. At this stage, pairwise comparisons of Cdm-0 and TAIR10.1 and A.arenosa and TAIR10.1 assemblies were made to see the structural changes in each genome relative to the reference version of A.thaliana.

A synteny plot was then constructed for the three genomes using the MCScan tool. MCScan allowed the identification of conserved regions and regions of rearrangements between the three genomes, which made it possible to see common and ecotype/species-specific structural differences.

## **Results**

**Pairwise synteny visualization**

Using dotplot visualization, rearrangements between Cdm-0 and A. arenosa assemblies were detected in comparison with TAIR10.1. While in the comparison of Cdm-0 with TAIR10.1 only deletions in centromere regions and one inversion of a small region were observed (red arrow in the left graph, Figure 1), multiple rearrangements were observed between A. arenosa and the reference version of A. thaliana (right graph, Figure 1), including translocations (blue arrows), inversions (red arrows), as well as regions that underwent both translocations and inversions (purple arrows).

*Figure 1. Pairwise synteny visualization (Ref vs Cdm and Ref vs A.arenosa)*
<img width="963" alt="Снимок экрана 2024-10-26 в 23 14 05" src="https://github.com/user-attachments/assets/027b92e9-322a-4b79-9b49-079af16e3144">

**Macrosynteny visualization** 

MCScan synteny plots showed a high degree of site conservation in the A. thaliana genomes (Cdm-0 and TAIR10.1). Except for deletions in chromosome centromere regions (which may be related to poor assembly in these regions), only a small site inversion is observed also near the centromere region of chromosome 881469 in Cdm-0 and 3075 in the reference sample (Figure 2). 

Many more rearrangements of different types were found when comparing A. arenosa and the reference version of A. thaliana. For example, inversion of a large region of chromosome 999457 of A. arenosa compared to 3075 A. thaliana, as well as multiple site translocations affecting chromosomes 999457, 999453, 999455, 999456 of A. arenosa. arenosa (Figure 2). These rearrangements were also observed in Figure 1.

*Figure 2. Macrosynteny visualization (Cdm vs Ref vs A.arenosa, before and after chromosome reordering)*
<img width="838" alt="Снимок экрана 2024-10-26 в 23 48 58" src="https://github.com/user-attachments/assets/d705255c-535b-41aa-95fd-f716384829e8">

**Microsynteny visualization**

<img width="769" alt="Снимок экрана 2024-10-27 в 00 17 54" src="https://github.com/user-attachments/assets/8fad3096-fd3e-4ba0-8b6a-8444eb02da5b">


## **Discussion**

The results of the analysis showed the presence of significant genomic rearrangements between Cdm-0 and A. arenosa assemblies compared to TAIR10.1. The detected inversions and deletions in the A. arenosa genome, as well as structural differences between TAIR10.1 and Cdm-0 ecotypes, may be a consequence of adaptation to specific environmental conditions. These differences may influence functional properties of genes, such as regulation of stress responses or metabolic processes, which are important for survival and reproduction of these plants under different conditions.

