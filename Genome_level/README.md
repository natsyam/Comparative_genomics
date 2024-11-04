# HW3. Comparative Genomics: *Arabidopsis thaliana* and *Arabidopsis arenosa*

### Introduction

In this report, we explore the genomic differences between *Arabidopsis thaliana* and *Arabidopsis arenosa*, two closely related species that exhibit significant ecological and morphological differences. *Arabidopsis thaliana* is a model organism widely used in plant genetics, while *Arabidopsis arenosa* is an allotetraploid species known for its unique adaptations to extreme environments. Comparative genomics can help uncover the structural and functional genomic variations that contribute to these adaptations. 

The main goals of this analysis were to:
1. Identify significant chromosomal rearrangements between the two genomes using JupiterPlot.
2. Analyze the repeat landscapes of *A. thaliana* ecotype Kyr-1 and *A. arenosa* using Kimura plots generated after repeat masking.
3. Visualize GC content, genes, and repeat density across the genomes using Circos, allowing us to examine correlations between these genomic features.

These analyses offer insights into the structural organization and evolutionary dynamics of the genomes and highlight differences that may be relevant to species-specific adaptations.

---

### 1. Comparative Genome Analysis of *Arabidopsis thaliana* and *Arabidopsis arenosa* Using JupiterPlot

We utilized JupiterPlot to visualize chromosomal rearrangements between the reference genomes of *A. thaliana* and *A. arenosa*. JupiterPlot helps to identify large-scale structural changes, such as inversions and translocations, by linking homologous regions between chromosomes (figure 1).

_Figure 1. Visualization of chromosomes of both species, with each color representing a specific chromosome (Colored are *Arabidopsis thaliana* reference genome)_

<img width="739" alt="Снимок экрана 2024-11-04 в 14 11 06" src="https://github.com/user-attachments/assets/07270c9a-a563-4437-97ea-a3aa9e7cbdaa">



**Significant Findings**:
   - **Inversion on Chromosome 1**: A large inversion was observed on *A. arenosa* chromosome NCBI_NC000927.4, which does not align with the homologous region in *A. thaliana*. This inversion could affect nearby genes by altering regulatory elements or gene orientation, potentially impacting gene expression.
   - **Translocation between Chromosome 2 and Chromosome 5**: Syntenic analysis showed evidence of a translocation event between *A. thaliana* chromosome NC000932.1 and *A. arenosa* chromosome LR999551. This rearrangement may disrupt local gene networks or facilitate adaptation through gene relocation.
   - **Duplication on Chromosome 3**: An apparent duplication in *A. arenosa* chromosome NCBI_NC000931.7 aligns with *A. thaliana* chromosome NC000933.5. Gene duplications are often associated with increased gene dosage or the emergence of novel functions, which could confer adaptive advantages.

   These rearrangements may play a role in the ecological differences observed between the two species by affecting gene function or expression patterns.

---

### 2. Analysis of Repeat Landscape Using Kimura Plots

We employed RepeatMasker and RepeatModeler to mask and classify repetitive sequences in *A. thaliana* ecotype Kyr-1 (figure 2) and *A. arenosa* (figure 3). Kimura plots allow visualization of the repeat landscapes, showing the diversity and age distribution of repeat elements based on substitution levels. The Kimura plots display various repeat classes, with substitution values indicating evolutionary age. Lower values (left side of the plot) represent recent insertions, while higher values (right side) indicate older, more diverged repeats.

_Figure 2. Visualization of repeat landscapes using Kimura Plots for *A. thaliana* ecotype Kyr-1_
<img width="1364" alt="Снимок экрана 2024-11-03 в 19 02 04" src="https://github.com/user-attachments/assets/a744f820-625a-46c8-a6c1-6388b1710fd8">

_Figure 3. Visualization of repeat landscapes using Kimura Plots for *A. arenosa*_
<img width="1141" alt="Снимок экрана 2024-11-04 в 14 43 12" src="https://github.com/user-attachments/assets/0716e000-f167-4a89-9f2d-756a49c3cf2a">


**Comparative Analysis**:
   - **Higher Proportion of Recent Repeats in *A. arenosa***: The *A. arenosa* shows a higher density of recent repeats, especially different variants of LTR, DNA and RC elements. This could indicate ongoing transpositional activity, which might influence genome plasticity and adaptability.
   - **Divergence in LINE Elements**: The Kimura plot for *A. arenosa* shows a more uniform distribution of LINE elements, with older repeats present in higher proportions than in *A. thaliana*. This suggests that *A. thaliana* may have accumulated LINE elements earlier in its evolutionary history, potentially contributing to genome stability.
   - **LTR Retrotransposons**: Both genomes show substantial representation of LTR retrotransposons, but the insertion patterns differ. The divergence of LTR elements in *A. arenosa* suggests a different transpositional history, potentially impacting genome evolution differently in each species.

   These differences in repeat landscapes reflect unique evolutionary pressures and histories, possibly contributing to species-specific adaptations.

---

### 3. Visualization of GC Content, Gene Density, and Repeat Density Using Circos

To gain a holistic view of the genome organization, we used Circos to visualize the distribution of GC content, gene density, and repeat density in *A. thaliana* and *A. arenosa*.

The Circos plot includes three main layers:
   - **Genes (dark gray)**: Represents the concentration of genes along the chromosomes.
   - **GC content (red)**: Indicates regions of higher or lower GC content.
   - **Repeat density (blue)**: Displays the distribution of repetitive elements.

_Figure 3. Visualization of GC-content, genes, and repeat density using Circos for *A. arenosa*_
<img width="726" alt="Снимок экрана 2024-11-04 в 14 07 16" src="https://github.com/user-attachments/assets/3ec8fd32-791a-45a2-a1af-a2df14f4b6bc">

**Results and Observations**:
   - **GC-Rich Regions Correlate with Gene-Rich Areas**: In both species, higher GC content often aligns with regions of higher gene density, suggesting that GC content may influence gene distribution and genome structure.
   - **Repeat Density Overlaps with Rearranged Regions**: Some areas of high repeat density coincide with chromosomal rearrangements observed in the JupiterPlot. This supports the idea that repetitive elements could facilitate structural rearrangements by promoting recombination.
   - **Divergent Patterns in Repeat Density**: The Circos plot reveals a more uniform distribution of repeats in *A. arenosa*, while *A. thaliana* shows clusters of higher repeat density. This difference might reflect varying evolutionary constraints or genome maintenance mechanisms in the two species.

   These observations provide insights into the genome organization and suggest that repeats and GC content are closely linked to genome structure and possibly to functional genomic elements.

---

### Conclusion
This comparative genomics analysis highlights key structural and functional differences between *Arabidopsis thaliana* and *Arabidopsis arenosa*. Chromosomal rearrangements, distinct repeat landscapes, and variations in GC content and gene density likely contribute to the ecological and physiological adaptations unique to each species. 

The findings from this study have broader implications for understanding the role of genome structure in adaptation and evolution. Future research could explore functional studies to validate the impacts of these structural variations on gene expression and phenotypic traits, advancing our knowledge of plant genomics and evolution.
