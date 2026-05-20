# CRISPR-Case9 knockout gene for tnf gene in human genome 
 To study TNF-knockout cell lines using gene editing tool CRISPR to understand exactly what roles TNF plays in body .
The workflow integrates public biological databases (**NCBI**) with premier web-based gRNA design platforms (**CHOPCHOP**, **CRISPOR**) and structural plasmid visualization software (**SnapGene**)[cite: 1] .


## 🛠️ Workflow Pipeline Step-by-Step

### **Step 1: Sequence Retrieval via NCBI**
* Navigate to the NCBI Nucleotide or Gene database[cite: 1].
* Search for the human *TNF* gene (Gene ID: 7124) and isolate the genomic, mRNA sequences[cite: 1].
* Export the sequence in FASTA format, identifying the locations of Exon 1, Exon 2, and Exon 3 to ensure the knockout targets the early coding region[cite: 1].

### **Step 2: Guide RNA Selection via CHOPCHOP** and CRISPOR**
* pasted the sequence in the software and foend the guide rna by verifing the efficiency and GC Content of the guide RNA
* labeled the selected PAM and gRNA in rhe snapegene for better visualisation
* Used diffrent Case proein such as Case9,Case12a.

  ### **Step 3: Off-Target Evaluation via CRISPOR**
* Cross-verify the top 3 candidate gRNAs from CHOPCHOP by pasting them into CRISPOR against the human genome[cite: 1].
* Evaluate the **MIT Off-Target Score** and **CFD Score** (higher is better, aiming for >80)[cite: 1].
* Select the single gRNA that maximizes on-target cutting efficiency while exhibiting zero predicted 0-mismatch or 1-mismatch off-target sites in the human exome[cite: 1].

# 📊 Comparative Analysis of Candidate gRNAs


<img width="1359" height="105" alt="image" src="https://github.com/user-attachments/assets/42c912ac-24a2-4b23-b264-c53f62eedc5a" />

## 🖼️ Visualizations & Figures
Here are the simulated layout map and targeting locations generated during this pipeline:

https://github.com/sunenabyadav-svg/CRISPR-Mini-Project-/blob/751be671d8c081c736c8e77780e7ef8dd18ed3fe/NCBI.png

https://github.com/sunenabyadav-svg/CRISPR-Mini-Project-/blob/4f025cd8ab4eb59187cf62d5995744347ac604ed/CHOPCHOP.png

https://github.com/sunenabyadav-svg/CRISPR-Mini-Project-/blob/1cdbc89d5c71d588472688e838dce630e03dc82b/snapgene.png

## 🏁 Conclusion & Selection
Based on the quantitative metrics derived from the multi-tool pipeline, **TNF-gRNA-01** is selected as the optimal candidate[cite: 1]. It possesses an ideal 55% GC content ensuring stable hybridization dynamics, a high efficiency score profile, and an excellent off-target safety profile across the hg38 human genome[cite: 1]. This blueprint is ready for wet-lab oligo ordering and subsequent plasmid transfection validation experiments[cite: 1]








