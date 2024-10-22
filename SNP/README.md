# **SNPs revealing in Arabidopsis**

## **Introduction**
 
**Arabidopsis** (*Arabidopsis thaliana*) is a model organism widely used in plant genetics research due to its manageable size, rapid life cycle, and ease of genetic manipulation. Within the comparative genomics, this plant may represent an important model for studying genomic adaptations to different environmental conditions.
 
One of the key mechanisms of plant adaptation to environmental stressors is the regulation of gene expression associated with the response to abiotic stresses such as cold and drought. One such gene is DREB1/CBF (Dehydration-Responsive Element-Binding protein 1), which plays an important role in the response to cold and drought by regulating the expression of other genes involved in cellular defence against stress.
 
Genomic studies show that although the genome is highly conserved in different Arabidopsis thaliana populations, there may be variations, such as single nucleotide polymorphisms (SNPs), that can influence the function of key genes and hence adaptation to environmental conditions.
 
This study compares the genome of Arabidopsis thaliana collected in Kyrgyzstan (ecotype Kyr-1, assembly GCA_036937335.1) and the reference genome (GCF_000001735.4, ecotype Columbia-0) to identify significant single nucleotide polymorphisms in the DREB1/CBF gene that may influence adaptation to different climatic conditions.
 
## **Methods**
 
The Kyr-1 ecotype genome assembly (GCA_036937335.1) was selected for analysis, representing a population adapted to Kyrgyz conditions. Columbia-0 ecotype (GCF_000001735.4), which inhabits more humid and stable climatic conditions, was used as a reference genome.
 
The BUSCO (Benchmarking Universal Single-Copy Orthologs) programme with a database for brassicales plants and the QUAST programme were used to assess the completeness and quality of the assembly.
 
Alignment of the Kyr-1 genome to the Columbia-0 reference genome was performed using the minimap2 tool, and the bcftools tool was used to identify single-nucleotide substitutions. SNPs in the DREB1/CBF and related gene regions were selected.
 
The online tool VEP (Variant Effect Predictor) and the UniProt database were used for functional annotation of SNPs. Protein structures were predicted using AlphaFold. The obtained substitutions were filtered according to their effects on protein structure and function (missense mutations with SIFT values < 0.05, which are labelled as deleterious, were selected). After that, variants with changes in polarity or charge of the amino acid were selected.
 
## **Results**
 
Evaluation with BUSCO and QUAST showed that the Kyr-1 genome assembly has high completeness (99.8%) for conserved plant genes, also high assembly quality, indicating that the assembly is of high quality and suitable for further analysis (Tables 1, 2 in the appendix).

The alignment and analysis with bcftools identified 72 SNPs in the DREB1/CBF gene region and in related genes. The number of missense mutations with SIFT values < 0.05 was 24, as well as one mutation marked as stop-gained (NC_003070.9:4385652-4385652, Figure 1). The tables below summarise the single nucleotide substitutions that resulted in a change in the polarity or charge of an amino acid in the protein.

*Table 3. Polarity changes*

| **Location**                     | **Allele** | **REF_ALLELE** | **Consequence**     | **SYMBOL**  | **Gene**     | **Protein_position** | **Amino_acids** | **Codons**  | **Existing_variation** | **SIFT**                       |
|----------------------------------|------------|----------------|----------------------|-------------|--------------|----------------------|------------------|-------------|-------------------------|---------------------------------|
| NC_003070.9:4298945-4298945     | A          | C              | missense_variant      | AT1G12630   | AT1G12630    | 17                   | P/T              | Ccg/Acg    | ENSVATH00020178        | deleterious(0)                 |
| NC_003070.9:4385656-4385656     | C          | T              | missense_variant      | SCRM2       | AT1G12860    | 300                  | I/T              | aTt/aCt    | ENSVATH01044293        | deleterious_low_confidence(0.04) |
| NC_003070.9:12238365-12238365   | A          | C              | missense_variant      | AT1G33760   | AT1G33760    | 141                  | P/Q              | cCg/cAg    | ENSVATH01168079        | deleterious(0)                 |
| NC_003075.7:7932430-7932430     | T          | C              | missense_variant      | AT4G13620   | AT4G13620    | 98                   | S/L              | tCg/tTg    | ENSVATH02818948        | deleterious(0.01)              |
| NC_003075.7:7933288-7933288     | A          | T              | missense_variant      | AT4G13620   | AT4G13620    | 384                  | F/Y              | tTt/tAt    | -                       | deleterious_low_confidence(0.03) |

*Table 4. Charge changes*

| **Location**                     | **Allele** | **REF_ALLELE** | **Consequence**     | **SYMBOL**  | **Gene**     | **Protein_position** | **Amino_acids** | **Codons**  | **Existing_variation** | **SIFT**                       |
|----------------------------------|------------|----------------|----------------------|-------------|--------------|----------------------|------------------|-------------|-------------------------|---------------------------------|
| NC_003070.9:4385013-4385013     | A          | G              | missense_variant      | SCRM2       | AT1G12860    | 86                   | D/N              | Gac/Aac    | ENSVATH01044277        | deleterious(0.01)              |
| NC_003071.7:16614852-16614852   | T          | C              | missense_variant      | HOS1        | AT2G39810    | 305                  | R/C              | Cgt/Tgt    | ENSVATH05686448        | deleterious(0)                 |

No significant SNPs were found directly in DREB1/CBF gene, but there are mutations in genes affecting them.

*Figure 1. Stop-gained variant illustration (gene SCRM2)*

![image](https://github.com/user-attachments/assets/4fa9b0fd-674d-4a44-929a-1bd5a99d97ea)

## **Discussion** 

In the SCRM2 gene (also known as SCREAM2), which encodes ICE2 (Inducer of CBF Expression 2), a bHLH family transcription factor involved in the cold acclimation pathway, several notable mutations were found. SCRM2 plays a key role in increasing resistance to freezing stress, especially following cold acclimatization. Overexpression of ICE2 has been shown to enhance this freezing tolerance.

Mutations leading to charge and polarity reversal of amino acids were found in SCRM2. However, the mutation affecting the change of amino acid polarity is located after the mutation leading to a stop codon and is likely not translated into the final protein, and the mutation with the change of amino acid charge does not affect any critical functional domains, and therefore, is unlikely to have a major impact on the protein's function.

One of the mutations identified in the SCRM2 gene leads to a premature stop codon, truncating the protein. It affects the bHLH domain, that plays a crucial role in stomatal development and function. It interacts with other transcription factors like SPCH, MUTE, and FAMA, which coordinate stomatal cell differentiation. Moreover, bHLH proteins often form heterodimers, allowing SCRM2 to regulate specific gene expression pathways related to stomatal development.

Stop-gained mutation affected the BHLH domain in the SCRM2 protein is reflected in Figure 2 by the loss of a section of the protein (the structure was predicted using alpha fold), which may negatively affect the function of this protein.

Since SCRM2 plays a key role in the regulation of stomata cell differentiation, loss of SCRM2 function due to changes in the bHLH domain could lead to absent or improper stomata formation, which would negatively affect the gas exchange and water balance of the plant. In addition, loss of part of the bHLH domain may impair the ability of SCRM2 to form heterodimers with other bHLH proteins such as SPCH and MUTE, making it difficult to activate target genes.

*Figure 2. SCRM2 predicted structure (changed one on the right)*

<img width="910" alt="Снимок экрана 2024-10-19 в 20 34 03" src="https://github.com/user-attachments/assets/f0e2defe-b189-4b71-a0c5-f267533aa26d">

In contrast, the HOS1 gene (High expression of osmotically responsive genes 1) encodes a protein with a RING finger motif and functions as an E3 ubiquitin-protein ligase. HOS1 negatively regulates cold response pathways by mediating the ubiquitination and degradation of ICE1, another critical transcription factor in cold acclimation. Overexpression of HOS1 results in increased sensitivity to freezing stress due to the repression of CBF (C-repeat binding factor) genes and their downstream targets. Interestingly, loss-of-function mutations in HOS1 cause an early flowering phenotype, as the plant exhibits constitutive vernalization, leading to reduced freezing tolerance without prior cold acclimation. 

In our case, the R/C amino acid change (charge change) observed in SCRM2, but does not affect critical functional regions. Therefore, it is presumed to have a minimal impact on the overall function of these proteins.

---

## **Supplementary information**

*Table 1. BUSCO Results from вataset Brassicales_odb10*
```
|Results from dataset brassicales_odb10                                                    |
-------------------------------------------------------------------------------------------
|C:99.8%[S:98.8%,D:1.0%],F:0.1%,M:0.1%,n:4596,E:1.0%                                       |
|4585    Complete BUSCOs (C)    (of which 47 contain internal stop codons)                 |
|4539    Complete and single-copy BUSCOs (S)                                               |
|46    Complete and duplicated BUSCOs (D)                                                  |
|5    Fragmented BUSCOs (F)                                                                |
|6    Missing BUSCOs (M)                                                                   |
|4596    Total BUSCO groups searched                                                       |
-------------------------------------------------------------------------------------------
```

*Table 2. QUAST Results* 

| **Assembly**                    | GCA_036937335.1         |
|----------------------------------|-------------------------|
| **# contigs (>= 50000 bp)**     | 5                       |
| **Total length (>= 50000 bp)**  | 136708680               |
| **Largest contig**              | 33123834                |
| **Total length**                | 136708680               |
| **GC (%)**                      | 36.47                   |
| **N50**                         | 25011401                |
| **N90**                         | 23018239                |
| **auN**                         | 28004272.4              |
| **L50**                         | 3                       |
| **L90**                         | 5                       |
| **# N's per 100 kbp**          | 1.48                    |
 


