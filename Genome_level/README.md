# HW3. Comparative Genomics: *Arabidopsis thaliana* and *Arabidopsis arenosa*

### Introduction

In this report, we explore the genomic differences between *Arabidopsis thaliana* and *Arabidopsis arenosa*, two closely related species that exhibit significant ecological and morphological differences. *Arabidopsis thaliana* is a model organism widely used in plant genetics, while *Arabidopsis arenosa* is an allotetraploid species known for its unique adaptations to extreme environments. Comparative analysis can help uncover the structural and functional genomic variations that contribute to these adaptations. 

The main goals of this analysis were to:
1. Identify significant chromosomal rearrangements between the two genomes using JupiterPlot.
2. Analyze the repeat landscapes of *A. thaliana* ecotype Kyr-1 and *A. arenosa* using Kimura plots generated after repeat masking.
3. Visualize GC content, genes, and repeat density in the *A. arenosa* genome using Circos, allowing us to examine correlations between these genomic features.

---

### Comparative genome analysis using JupiterPlot

JupiterPlot was utilized to visualize chromosomal rearrangements between the reference genomes of *A. thaliana* and *A. arenosa*. JupiterPlot helps to identify large-scale structural changes, such as inversions and translocations, by linking homologous regions between chromosomes (figure 1).

_Figure 1. Visualization of chromosomes of both species, with each color representing a specific chromosome (Colored are *Arabidopsis thaliana* reference genome)_

<img width="739" alt="Снимок экрана 2024-11-04 в 14 11 06" src="https://github.com/user-attachments/assets/07270c9a-a563-4437-97ea-a3aa9e7cbdaa">

Synteny analysis showed an inversion between chromosomes NC003070.9 of *A. thaliana* and LR999451.1 of *A. arenosa*, but since this inversion affected an entire arm of the chromosome, this rearrangement event is unlikely to have had major consequences. In addition, multiple translocations were observed between *A. thaliana* chromosome NC003071.7 and *A. arenosa* chromosomes: LR999453.1, LR999455.1. This rearrangement may disrupt local gene networks or facilitate adaptation through gene relocation. 

Also of interest are translocations of chromosome regions involving chromosomes NC003075.7 and NC003076.8 of *A. thaliana*, which form mixed chromosomes LR999456.1, LR999457.1 of *A. arenosa*. However, as in the case of inversion, these rearrangements affect the whole arms of the affected chromosomes and therefore it is difficult to speak about the influence of these translocations. Worth noting also aligns plastid DNA NC_000932.1 to LR999452.1

These rearrangements may play a role in the ecological differences observed between the two species by affecting gene function or expression patterns.

---

### Analysis of Repeat Landscape using Kimura Plots

RepeatMasker and RepeatModeler were employed to mask and classify repetitive sequences in *A. thaliana* ecotype Kyr-1 (figure 2) and *A. arenosa* (figure 3). Kimura plots allow visualization of the repeat landscapes, showing the diversity and age distribution of repeat elements based on substitution levels. The Kimura plots display various repeat classes, with substitution values indicating evolutionary age. Lower values (left side of the plot) represent recent insertions, while higher values (right side) indicate older, more diverged repeats.

_Figure 2. Visualization of repeat landscapes using Kimura Plots for *A. thaliana* ecotype Kyr-1_
<img width="1364" alt="Снимок экрана 2024-11-03 в 19 02 04" src="https://github.com/user-attachments/assets/a744f820-625a-46c8-a6c1-6388b1710fd8">

_Figure 3. Visualization of repeat landscapes using Kimura Plots for *A. arenosa*_
<img width="1141" alt="Снимок экрана 2024-11-04 в 14 43 12" src="https://github.com/user-attachments/assets/0716e000-f167-4a89-9f2d-756a49c3cf2a">

A distinctive feature that is immediately apparent is the peak of repeats of unknown origin in *A. thaliana*, but otherwise the repeat landscapes remain similar, which becomes apparent when the plots are brought to the same scale.  Both species show a higher density of recent repeats, especially of different LTR variants, DNA repeats and RC elements. This may indicate ongoing transposition activity that may influence genome plasticity and adaptability. Both genomes show substantial representation of LTR retrotransposons.

---

### Visualization of GC-content, Genes and Repeat Density using Circos

To gain a holistic view of the genome organization, Circos tool was used to visualize the distribution of GC-content, genes, and repeat density in *A. arenosa*.

_Figure 3. Visualization of GC-content, genes, and repeat density using Circos for *A. arenosa*_
<img width="726" alt="Снимок экрана 2024-11-04 в 14 07 16" src="https://github.com/user-attachments/assets/3ec8fd32-791a-45a2-a1af-a2df14f4b6bc">

Visualization of the Circos plot provides insight into gene density, GC content, and repeat density in *Arabidopsis arenosa* chromosomes. 

Gene density (dark gray track) is relatively constant across most of the genome, but in some regions genes are missing. These gene-poor regions are probably associated with centromeric regions.

GC content (red track) shows noticeable dips in these gene-poor regions, supporting the idea that centromeric regions are not only gene-poor but also have lower GC composition. This is consistent with literature data obtained in various plant genomes.

The blue track representing repeat density also shows a decrease in these putative centromeric regions. In many genomes, centromeric regions contain unique repetitive elements rather than a high density of transposable elements, which may explain the observed decrease in repeat density in these regions. 

Centromeres are known to have a unique chromatin structure enriched with specific repetitive elements that may differ from the repeats scattered throughout the rest of the genome. 

---

### Conclusion

Comparative genomic analysis between *Arabidopsis thaliana* and *Arabidopsis arenosa* revealed notable structural differences that may underlie their different ecological adaptations. The chromosomal rearrangements identified using JupiterPlot, particularly inversions and translocations, emphasize the plasticity of the genome in these species. While some of these rearrangements span entire branches of chromosomes, potentially minimizing functional disruption, others may have contributed to adaptive evolution by altering gene locations and regulatory landscapes.

Analysis of the repeat landscape using Kimura plots also shows that both species exhibit a similar composition of repetitive elements, among which recent insertions of LTR retrotransposons and DNA repeats predominate. This predominance of recent transposon activity suggests that the genomes of both species remain dynamic, with ongoing transpositions contributing to genomic variability and potentially enhancing adaptability.

Visualization of the Circos plot for *A. arenosa* provides additional insight into the structural organization of the genome, highlighting correlations between gene density, GC content, and repeat density. The observed gene-poor regions with low GC content likely correspond to centromeric regions that exhibit particular compositional characteristics. These centromeric regions are also marked by a lower repeat density in *A. arenosa*, consistent with the presence of specialized repeats rather than abundant transposable elements.

---
### Supplementary information


_Table 1. Repeats presence in *A. thaliana* Kyr-1 ecotype_

| Category             | Number of Elements | Length Occupied (bp) | Percentage of Sequence |
|----------------------|--------------------|-----------------------|------------------------|
| **Retroelements**    | 7472               | 6,795,252            | 4.97%                  |
| SINEs                | 172                | 28,405               | 0.02%                  |
| Penelope             | 0                  | 0                    | 0.00%                  |
| LINEs                | 2204               | 1,177,783            | 0.86%                  |
| CRE/SLACS            | 0                  | 0                    | 0.00%                  |
| L2/CR1/Rex           | 0                  | 0                    | 0.00%                  |
| R1/LOA/Jockey        | 0                  | 0                    | 0.00%                  |
| R2/R4/NeSL           | 0                  | 0                    | 0.00%                  |
| RTE/Bov-B            | 0                  | 0                    | 0.00%                  |
| L1/CIN4              | 2204               | 1,177,783            | 0.86%                  |
| LTR elements         | 5096               | 5,589,064            | 4.09%                  |
| BEL/Pao              | 0                  | 0                    | 0.00%                  |
| Ty1/Copia            | 1282               | 973,841              | 0.71%                  |
| Gypsy/DIRS1          | 3724               | 4,608,320            | 3.37%                  |
| Retroviral           | 90                 | 6,903                | 0.01%                  |
| **DNA transposons**  | 3361               | 2,248,334            | 1.64%                  |
| hobo-Activator       | 138                | 80,544               | 0.06%                  |
| Tc1-IS630-Pogo       | 250                | 46,580               | 0.03%                  |
| En-Spm               | 0                  | 0                    | 0.00%                  |
| MULE-MuDR            | 1944               | 1,369,920            | 1.00%                  |
| PiggyBac             | 0                  | 0                    | 0.00%                  |
| Tourist/Harbinger    | 166                | 52,831               | 0.04%                  |
| Other (Mirage, P-element, Transib) | 0  | 0                    | 0.00%                  |
| **Rolling-circles**  | 1573               | 736,793              | 0.54%                  |
| **Unclassified**     | 34,696             | 22,539,195           | 16.49%                 |
| **Total interspersed repeats** | -       | 31,582,781           | 23.10%                 |
| Small RNA            | 358                | 789,478              | 0.58%                  |
| Satellites           | 0                  | 0                    | 0.00%                  |
| Simple repeats       | 34,710             | 1,397,676            | 1.02%                  |
| Low complexity       | 8588               | 413,831              | 0.30%                  |

---

_Table 2. Repeats presence in *A. arenosa*_

| Category             | Number of Elements | Length Occupied (bp) | Percentage of Sequence |
|----------------------|--------------------|-----------------------|------------------------|
| **Retroelements**    | 9762               | 8,103,013            | 5.41%                  |
| SINEs                | 34                 | 2,639                | 0.00%                  |
| Penelope             | 0                  | 0                    | 0.00%                  |
| LINEs                | 5073               | 2,753,256            | 1.84%                  |
| CRE/SLACS            | 0                  | 0                    | 0.00%                  |
| L2/CR1/Rex           | 0                  | 0                    | 0.00%                  |
| R1/LOA/Jockey        | 0                  | 0                    | 0.00%                  |
| R2/R4/NeSL           | 0                  | 0                    | 0.00%                  |
| RTE/Bov-B            | 0                  | 0                    | 0.00%                  |
| L1/CIN4              | 5073               | 2,753,256            | 1.84%                  |
| LTR elements         | 4655               | 5,347,118            | 3.57%                  |
| BEL/Pao              | 29                 | 17,477               | 0.01%                  |
| Ty1/Copia            | 2661               | 2,161,773            | 1.44%                  |
| Gypsy/DIRS1          | 1965               | 3,167,868            | 2.12%                  |
| Retroviral           | 0                  | 0                    | 0.00%                  |
| **DNA transposons**  | 2196               | 1,144,507            | 0.76%                  |
| hobo-Activator       | 480                | 185,785              | 0.12%                  |
| Tc1-IS630-Pogo       | 0                  | 0                    | 0.00%                  |
| En-Spm               | 0                  | 0                    | 0.00%                  |
| MULE-MuDR            | 964                | 588,404              | 0.39%                  |
| PiggyBac             | 0                  | 0                    | 0.00%                  |
| Tourist/Harbinger    | 430                | 199,500              | 0.13%                  |
| Other (Mirage, P-element, Transib) | 0  | 0                    | 0.00%                  |
| **Rolling-circles**  | 3150               | 1,095,400            | 0.73%                  |
| **Unclassified**     | 56,650             | 18,172,927           | 12.14%                 |
| **Total interspersed repeats** | -       | 27,420,447           | 18.32%                 |
| Small RNA            | 315                | 164,743              | 0.11%                  |
| Satellites           | 67                 | 36,808               | 0.02%                  |
| Simple repeats       | 45,457             | 1,806,479            | 1.21%                  |
| Low complexity       | 10,792             | 528,455              | 0.35%                  |
