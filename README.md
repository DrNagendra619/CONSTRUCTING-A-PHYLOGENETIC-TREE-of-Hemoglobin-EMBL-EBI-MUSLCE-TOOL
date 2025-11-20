# CONSTRUCTING-A-PHYLOGENETIC-TREE-of-Hemoglobin-EMBL-EBI-MUSLCE-TOOL
CONSTRUCTING-A-PHYLOGENETIC-TREE-of-Hemoglobin-EMBL-EBI-MUSLCE-TOOL
Hemoglobin Chain Phylogenetic Analysis (MUSCLE)

This repository contains the results of a multiple sequence alignment (MSA) and phylogenetic tree construction for a set of α- and β-like Hemoglobin protein chains, performed using the MUSCLE (v3.8) tool on the EMBL-EBI Job Dispatcher.

The analysis uses the same 11 Hemoglobin protein sequences as the Clustal Omega analysis, providing an independent comparative view of their evolutionary relationships.

📁 Repository Contents
Filename,Description,Source
muscle-I20250718-063307-0344-23525757-p1m.sequence,Input FASTA File containing 11 Hemoglobin chain protein sequences (PDB IDs with chain designators).,Input
muscle-I20250718-063307-0344-23525757-p1m.aln-clustalw / Muscle _ EMBL-EBI ALIGNMENTS .pdf,"Multiple Sequence Alignment (MSA) in CLUSTALW format, showing aligned residues and conservation scores.",Output
muscle-I20250718-063307-0344-23525757-p1m.pim,"Percent Identity Matrix (PIM), detailing pairwise sequence similarity percentages.",Output
muscle-I20250718-063307-0344-23525757-p1m.phylotree,Newick format of the Phylogenetic Tree (Guide Tree).,Output
Hemoglobin PHLYOGENETIC TREE RADIAL MUSCLE TOOL.png,Graphical representation of the Phylogenetic Tree (Radial View).,Output
Hemoglobin PHLYOGENETIC TREE PHYLOGRAM MUSCLE TOOL.png,Graphical representation of the Phylogenetic Tree (Rectangular Phylogram).,Output
Multiple Sequence Alignment (MSA) & Conservation

The MUSCLE algorithm produced an MSA that highlighted key conservation patterns:

    Identical Residues (∗): Found in the heme-binding pocket region, specifically around the proximal Histidine (often conserved in Globins).

Highly Conserved Residues (:): Several other key structural and functional regions show strong similarity across most Hemoglobin chains.

Key Sequence Identities (from PIM)

The Percent Identity Matrix confirms the clustering observed in the phylogenetic tree, with high pairwise identity within the two major groups
Group,Sequences,Pairwise Identity Range (Max % Identity)
Alpha-like,"1HDA_1, 1A3N_1, 2D5X_1",87.94% to 100% 
Beta-like,"1HDA_2, 1A3N_2, 2D5X_2",81.38% to 84.14% 
Divergent,1VHB_1 vs. All others,≈ 15.79% to 17.78% 
Phylogenetic Tree Analysis

The MUSCLE phylogenetic tree (UPGMB method) successfully clustered the Hemoglobin chains into three major groups, consistently reflecting known Globin family distinctions:

    Alpha Chain Clade (Closer Group):

        Sequences from Human (1A3N_1), Cattle (1HDA_1), and Horse (2D5X_1) cluster tightly, confirming high conservation among mammalian α-chains.

The Chicken α-chain (1HBR_1) is an outlier to the main mammalian group, suggesting greater evolutionary distance.

Beta Chain Clade (Closer Group):

    Sequences from Human (1A3N_2), Cattle (1HDA_2), and Horse (2D5X_2) cluster closely, indicating they are the β-chain counterparts.

The Chicken β-chain (1HBR_2) is an outlier to this mammalian group, consistent with the α-chain result.

Highly Divergent Clade (Outgroups):

    Vitreoscilla stercoraria Hemoglobin (1VHB_1) and the Mustelus griseus (Shark) chains (1GCW_1 and 1GCW_2) appear on the longest branches, confirming they are the most evolutionarily distant sequences compared to the mammalian/avian α and β chains.

1VHB_1 (a bacterial Globin) has the longest branch length (0.49461), correctly identifying it as the most distantly related protein in the dataset.

🛠️ Methods and Citation

Tool Execution

    Program: MUSCLE (Multiple Sequence Comparison by Log-Expectation).

Version: v3.8.425.

Distance Method (2): PctIdKimura.

Clustering Method: UPGMB (Unweighted Pair Group Method with Arithmetic mean).

Job Title: HEMO CHAINS MUSLCE TOOL.

Citation

If you utilize this analysis in your work, please cite the MUSCLE publication:

    Edgar, R.C. (2004). MUSCLE: multiple sequence alignment with high accuracy and high throughput. Nucleic Acids Research, 32(5): 1792-97.
