# Muscle-Contractility-RYR2

## A

**Assignment number:** 22

**Gene:** RYR2

**Matching NP_protein accession:** NP_001026.2

**ClinVar ID:** 201214

## B. Research Questions

**1. What does your assigned gene encode, and how does this protein contribute to muscle function?**

The RYR2 gene provides instructions for making the ryanodine receptor 2 (RyR2), a calcium-release channel found in the sarcoplasmic reticulum of cardiac muscle cells. This channel releases stored calcium into the cell, which helps trigger heart muscle contraction. Calcium is then removed from the cytoplasm or returned to storage, allowing the heart muscle to relax (Gao et al., 2026)

**2. What was the exact protein accession and length retrieved with R?**

The protein accession retrieved using R was NP_001026.2, which corresponds to the human RYR2 protein. Based on the retrieved FASTA sequence, the protein contains 4,967 amino acids.

**3. What did the amino-acid composition chart show? What can it NOT tell you?**

The amino-acid composition chart showed the number of times each of the 20 standard amino acids appeared in the RYR2 protein sequence. Leucine (L) was the most abundant amino acid, followed by glutamic acid (E) and serine (S). Tryptophan (W) was the least abundant in the chart. The chart helped me understand the amino-acid composition of the protein. However, it cannot explain the complete three-dimensional structure of RYR2 or prove how the assigned mutation affects its function.

**4. What is your fixed ClinVar variant, and what is its current classification and evidence strength?**

My assigned variant is RYR2 NM_001035.3.1258C>T (p.Arg420Trp), with ClinVar Variation ID 201214. It is a missense variant because the change in DNA results in the replacement of arginine with tryptophan at amino-acid position 420. The current ClinVar aggregate classification is Pathogenic, with 12 of 13 submissions contributing to this classification and no conflicts among the contributing submissions. The evidence includes reports of the variant in affected individuals and families, experimental studies showing altered calcium release, and studies in mice showing increased susceptibility to arrhythmias. These findings provide substantial evidence supporting its pathogenic classification.

**5. What is the scientifically supported mechanism linking this variant to muscle function, and what
remains uncertain?**

The RYR2 p.Arg420Trp mutation changes the amino acid arginine to tryptophan at position 420 of the RyR2 protein. Changes in RYR2 can affect how the channel releases calcium from the sarcoplasmic reticulum. Abnormal calcium release may cause irregular electrical activity in heart cells and increase the risk of heart rhythm disorders, such as catecholaminergic polymorphic ventricular tachycardia (CPVT) (Woll & Van Petegem, 2022). However, further studies are needed to fully explain the specific molecular effects of the p.Arg420Trp mutation.

**6. What additional experiment would help test the proposed mechanism?**

One useful experiment would be calcium imaging in cardiac muscle cells expressing the normal RYR2 protein and the p.Arg420Trp variant. The calcium signals could be measured and compared under the same experimental conditions. If the variant causes abnormal calcium release, differences in the calcium signals may be observed between the two groups. This experiment would help test how the variant affects calcium regulation and cardiac muscle function.

## C. Exact numbered methods including R command

**1. Project Setup**

<img width="419" height="191" alt="image" src="https://github.com/user-attachments/assets/f82af635-8ca2-4721-89be-55a872506059" />

The R project folder Muscle_Contractility_RYR2 that contains the analysis.R script and the data, results, and figures subfolders, with packages installed once and the setup code run in each new R session.

**2. Retrieving of the human RYR2 gene record from NCBI using R.

<img width="390" height="329" alt="image" src="https://github.com/user-attachments/assets/c8f713c0-2d0b-4e4b-88c8-790e9835bd33" />

<img width="339" height="97" alt="image" src="https://github.com/user-attachments/assets/715eda52-d8b2-46f8-9413-0c3f6e8406d1" />

Retrieval of the human NCBI Gene record for the selected gene, RYR2, using R code with the exact gene symbol and human taxonomy ID (9606). The code identifies the numeric Gene ID, official gene name, and chromosome. 

**3. Retrieving of the corresponding protein sequence using the assigned transcript.**

<img width="500" height="302" alt="image" src="https://github.com/user-attachments/assets/baf260a4-a2b4-485d-8a44-d7eb367113df" />

<img width="489" height="87" alt="image" src="https://github.com/user-attachments/assets/f68636d4-9b17-49e3-a451-9395ba80d47a" />

The transcript NM_001035.3 was used to identify its corresponding protein record in NCBI. The protein sequence was downloaded in FASTA format, saved in the data folder, and its accession number was recorded in the results folder.

**4. Examining protein length and composition in R**

<img width="512" height="292" alt="image" src="https://github.com/user-attachments/assets/85f2c6ec-78a7-4699-87fd-3a59cf8603c2" />

The protein sequence was analyzed in R to determine its length and count the 20 standard amino acids. The amino-acid counts were saved as a CSV file, and a bar chart was generated to show their composition and identify the three most abundant amino acids.

**5. ClinVar Variant Documentation**

<img width="385" height="434" alt="image" src="https://github.com/user-attachments/assets/4fc8108b-1e74-4875-b5cb-7a2f2c43c642" />

The assigned RYR2 variant, NM_001035.3:c.1258C>T (p.Arg420Trp), was examined in ClinVar. Its variant type, pathogenic classification, amino-acid change, and supporting information were recorded for documentation.

**6. Producing a Protein Position Visualization**

<img width="521" height="324" alt="image" src="https://github.com/user-attachments/assets/5ef1ba6b-bc0f-4941-8f0e-f8fdcd2aff4b" />

The reference protein was visualized in R, showing the amino acid position of the assigned variant (p.Arg420Trp) along the protein sequence. The figure was saved as a PNG file for documentation.

**7. Molecular mechanism**

The RYR2 gene provides instructions for producing ryanodine receptor 2, a calcium-release channel found in the sarcoplasmic reticulum of cardiac muscle cells. This channel releases calcium ions into the cytoplasm, allowing the heart muscle to contract. Proper regulation of calcium release is important for normal heart contraction and relaxation. The assigned variant, NM_001035.3:c.1258C>T (p.Arg420Trp), is a missense variant that changes the amino acid arginine to tryptophan at position 420 of the RYR2 protein. ClinVar currently classifies this variant as pathogenic. Experimental studies have shown increased calcium release through RYR2 channels and altered calcium signaling. Studies in knock-in mice also found increased susceptibility to abnormal heart rhythms. These findings support the variant's effect on protein function, although the exact molecular changes should not be assumed to explain every clinical outcome. RYR2 gene → production of the RYR2 calcium channel → regulation of calcium release in cardiac muscle → p.Arg420Trp amino acid change → abnormal calcium release and signaling → increased susceptibility to irregular heart rhythms. Calcium imaging could be used to compare calcium release in cardiac cells expressing normal RYR2 and cells expressing the p.Arg420Trp variant. The calcium signals could be measured and compared to determine whether the variant causes changes in calcium release during muscle contraction. 

**8. Make the complete workflow and final results available on GitHub**

The GitHub repository, Muscle-Contractility-GENE, contains the complete workflow and results of the RYR2 gene analysis, including the R script, protein FASTA sequence, gene summary, protein accession, amino acid composition, and generated figures. The README.md file provides the assignment details, research question, step-by-step methods, results, variant interpretation, limitations, proposed validation experiment, and database references to help other students reproduce the analysis. 

## D. Results/Figures

**Table 1.** Amino acid composition of the RYR2 protein showing the count of each amino acid residue in the analyzed protein sequence.

<img width="82" height="210" alt="image" src="https://github.com/user-attachments/assets/f87da110-d832-497d-b262-477211f27cf3" />

<img width="2400" height="1500" alt="01_amino_acid_composition" src="https://github.com/user-attachments/assets/0a52a9af-ba43-4fe0-b327-688631afabcc" />

**Figure 1.** Amino acid composition of the RYR2 protein showing the number of residues for each of the 20 standard amino acids. Leucine (L) was the most abundant amino acid, while tryptophan (W) was the least abundant in the analyzed protein sequence. 

<img width="2400" height="750" alt="02_variant_position" src="https://github.com/user-attachments/assets/680248bc-c78e-4342-8187-1daa294bd391" />

**Figure 2.** Visualization of the RYR2 reference protein sequence showing the position of the assigned variant, p.Arg420Trp, at amino acid 420, where arginine is replaced by tryptophan. 

## E. Variant Interpretation

The RYR2 variant p.Arg420Trp (NM_001035.3:c.1258C>T) is a missense variant that changes the amino acid arginine to tryptophan at position 420 of the RYR2 protein. This change replaces a positively charged amino acid with one that has different chemical properties, which may affect protein function. ClinVar classifies this variant as pathogenic (Variation ID: 201214). Experimental studies have shown that the variant can increase calcium release through RYR2 channels and disrupt normal calcium signaling. It has also been reported in individuals with catecholaminergic polymorphic ventricular tachycardia (CPVT), a condition that can cause abnormal heart rhythms, and sudden unexplained death. These findings support the interpretation that p.Arg420Trp can affect RYR2 function and contribute to heart rhythm disorders (NCBI ClinVar, 2026).

## F. Limitations and a possible validation experiment

One limitation of this analysis is that it mainly relies on online databases and protein sequence analysis. Although these methods help identify the p.Arg420Trp variant in the RYR2 protein, they cannot fully explain how the change affects calcium release in heart muscle cells. The results also depend on the information available from previous studies. To further investigate the variant, calcium release could be compared between cardiac cells with the normal RYR2 protein and those with the variant. This would help determine whether the amino acid change affects the protein's function. 

## G. Database links, accession versions, access dates, and citations

| Database/Resource | Accession or Record ID | Link | Access Date |
|---|---|---|---|
| NCBI Gene | RYR2 (Human) | [NCBI Gene](https://www.ncbi.nlm.nih.gov/datasets/gene/6262/) | October 27, 2026 |
| NCBI Nucleotide | NM_001035.3 | [RYR2 mRNA Sequence](https://www.ncbi.nlm.nih.gov/nuccore/NM_001035.3) | October 27, 2026 |
| NCBI Protein | NP_001026.2 | [RYR2 Protein Sequence](https://www.ncbi.nlm.nih.gov/protein/NP_001026.2) | October 27, 2026 |
| ClinVar | Variation ID 201214 | [RYR2 Variant Record](https://www.ncbi.nlm.nih.gov/clinvar/variation/201214/) | October 27, 2026 |

## H. Discussion

The analysis of the RYR2 gene focused on examining its reference protein sequence and amino acid composition using bioinformatics tools and R programming. The reference transcript, NM_001035.3, and its corresponding protein sequence were retrieved from the National Center for Biotechnology Information (NCBI). The protein sequence was analyzed in R to determine its length and count the 20 standard amino acids. The results showed that leucine (L) was the most abundant amino acid, with 555 residues, followed by glutamic acid (E), with 410 residues, and serine (S), with 353 residues. In contrast, tryptophan (W) was the least abundant, with 57 residues. These results were presented in a table and bar graph to show the distribution of amino acids in the RYR2 protein.
The protein sequence was also visualized to show the location of the assigned variant at amino acid position 420. This visualization helped identify the specific position within the protein sequence for reference in the analysis. The use of R programming made it easier to process the protein sequence, count amino acid residues, and generate figures for presenting the results. Organizing the outputs into tables, graphs, and text files also made the analysis easier to review and reproduce.
Throughout the activity, online databases such as NCBI Gene, NCBI Nucleotide, NCBI Protein, and ClinVar were used to obtain gene, transcript, protein, and variant information. These resources provided the reference records needed to support the analysis and document the assigned gene. The results and figures were organized into a GitHub repository containing the R script, protein FASTA file, summary files, amino acid composition table, and generated figures. The README file documents the workflow and provides instructions that other students can follow to reproduce the analysis.
Overall, this activity demonstrated how bioinformatics tools and databases can be used to examine a gene and its protein sequence. It also provided practical experience in using R to analyze biological data, generate visual representations, and organize research outputs. The activity highlighted the importance of accurate data retrieval, proper documentation, and reproducible methods in biological research.

## Scientific Refereces

Gao, K., Wang, W., Ling, Y., Li, B., Xing, C., Li, N., Yin, X., Tao, L., Li, X., Qiu, J., Wang, X., & Wei, J. (2026). Structural and Functional Regulation of RyR2 in Cardiac Calcium Handling and Arrhythmogenesis. Biomedicines, 14(3), 662. https://doi.org/10.3390/biomedicines14030662

Calcium-release channels: Structure and function of IP3 receptors and ryanodine receptors | physiological reviews | american physiological society. (n.d.). https://journals.physiology.org/doi/full/10.1152/physrev.00033.2020 

U.S. National Library of Medicine. (n.d.). Checking your browser - recaptcha. National Center for Biotechnology Information. https://www.ncbi.nlm.nih.gov/clinvar/variation/201214/ 

