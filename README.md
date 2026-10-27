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
