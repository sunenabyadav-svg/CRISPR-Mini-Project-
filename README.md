# CRISPR-Case9 knockout gene for tnf gene in human genome 
 To study TNF-knockout cell lines using gene editing tool CRISPR to understand exactly what roles TNF plays in body .

The workflow integrates public biological databases (**NCBI**) with premier web-based gRNA design platforms (**CHOPCHOP**, **CRISPOR**) and structural plasmid visualization software (**SnapGene**)[cite: 1] .

---

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

* 
