# Exploring Lysosomal Enzymes Using NCBI and R: HYAL1

## 1. Enzyme and Gene Information

- **Gene symbol:** HYAL1
- **Enzyme name:** Hyaluronidase-1
- **Organism:** *Homo sapiens* (human)
- **NCBI Protein Accession:** NP_695013.1
- **NCBI Protein Record:** https://www.ncbi.nlm.nih.gov/protein/NP_695013.1

HYAL1 encodes hyaluronidase-1, a lysosomal enzyme that breaks down hyaluronan, a major component of the extracellular matrix. This process helps the body degrade and recycle hyaluronan.

## 2. Objective

The objective of this activity was to retrieve a human lysosomal enzyme protein sequence from NCBI, analyze its amino acid composition and potential N-linked glycosylation motifs using R, and publish the results in a GitHub repository.

## 3. Methods

The human HYAL1 protein sequence was retrieved from NCBI using accession NP_695013.1. The R script used the `rentrez` and `ggplot2` packages to retrieve and analyze the protein sequence, calculate amino acid counts and percentages, identify potential N-linked glycosylation motifs, and generate figures.

## 4. Results

The HYAL1 protein sequence analyzed contains **435 amino acids** and **three potential N-linked glycosylation motifs**.

The most abundant amino acids were:

- Alanine (A): 46 residues (10.57%)
- Leucine (L): 46 residues (10.57%)
- Glycine (G): 35 residues (8.05%)
- Proline (P): 33 residues (7.59%)
- Glutamine (Q): 28 residues (6.44%)

The three potential N-linked glycosylation motifs identified were:

- Position 99: NAS
- Position 216: NYT
- Position 350: NVT

These sequences match the N-X-S/T motif pattern. However, identifying a potential motif does not confirm that glycosylation actually occurs.

## 5. Figures

### Figure 1. Amino Acid Composition of the HYAL1 Protein

![Amino acid composition of HYAL1](lysosomal-enzyme-HYAL1/figures/HYAL1_amino_acid_composition.png)
This figure shows the amino acid composition of the human HYAL1 protein sequence, including the relative abundance of its amino acid residues.

### Figure 2. Potential N-Linked Glycosylation Motifs in HYAL1

![Potential N-linked glycosylation motifs in HYAL1](lysosomal-enzyme-HYAL1/figures/HYAL1_potential_N_glycosylation.png)
This figure shows the positions of the three potential N-linked glycosylation motifs identified in the HYAL1 protein sequence.

## 6. Guide Questions and Answers

### 1. What does your enzyme normally break down inside lysosomes?

HYAL1 encodes hyaluronidase-1, a lysosomal enzyme that breaks down hyaluronan into smaller fragments. Hyaluronan is a component of the extracellular matrix, and its degradation contributes to the recycling of this material.

### 2. What is the total length of your protein, and which amino acids are most common?

The human HYAL1 protein sequence analyzed contains 435 amino acids. Alanine (A) and leucine (L) are the most abundant amino acids, with 46 residues each (10.57%). They are followed by glycine (G), with 35 residues (8.05%); proline (P), with 33 residues (7.59%); and glutamine (Q), with 28 residues (6.44%).

### 3. How many potential N-glycosylation motifs did you find? Where are they located?

Three potential N-linked glycosylation motifs were identified: NAS at position 99, NYT at position 216, and NVT at position 350. These sequences follow the N-X-S/T pattern, where X can be any amino acid except proline. These are predicted sites and do not confirm actual glycosylation.

### 4. Why can glycosylation matter for lysosomal proteins? Does finding a motif prove the protein is glycosylated?

Glycosylation can help proteins fold correctly, maintain stability, and support their transport and function. Certain carbohydrate modifications also help direct lysosomal enzymes to lysosomes. However, finding an N-X-S/T motif does not prove that a carbohydrate group is attached to the protein. Sequence analysis also cannot confirm whether the protein carries a mannose-6-phosphate tag.

### 5. What could happen in the cell if your enzyme did not work properly?

If HYAL1 does not function properly, hyaluronan degradation can be impaired, resulting in the accumulation of hyaluronan or its fragments. HYAL1 deficiency is associated with mucopolysaccharidosis type IX, a rare lysosomal storage disorder. This illustrates how impaired lysosomal enzyme function can disrupt normal cellular and tissue processes.

## 7. Repository Contents

- `lysosomal_enzyme_analysis.R` — R script used for the analysis
- `data/HYAL1.fasta` — retrieved HYAL1 protein sequence
- `results/HYAL1_summary.csv` — protein length and potential motif count
- `results/HYAL1_amino_acid_counts.csv` — amino acid counts and percentages
- `results/HYAL1_motif_positions.csv` — predicted motif positions and sequences
- `figures/HYAL1_amino_acid_composition.png` — amino acid composition figure
- `figures/HYAL1_potential_N_glycosylation.png` — potential glycosylation motif figure

## 8. Conclusion

The analysis of the human HYAL1 protein identified a sequence length of 435 amino acids and three potential N-linked glycosylation motifs. Alanine and leucine were the most abundant amino acids. Using NCBI and R made it possible to retrieve the protein sequence, characterize its amino acid composition, identify potential sequence motifs, and visualize the results. These findings describe sequence features but do not directly measure protein glycosylation or enzyme activity.
