# Ensembl Biomart Project
 
Finding Mouse Homologs of Human Genes using Ensembl BioMart
Background: Homologous genes are genes that share a common evolutionary ancestor. Between human and mouse, homologous genes often perform similar functions. Ensembl BioMart provides a comprehensive database of gene homology relationships and allows programmatic access to this information.

Task:
Write a Python script to find the mouse orthologs of specific human genes using Ensembl BioMart and supporting tools.

Data Source:

Primary: Ensembl BioMart

Dataset: Human genes (GRCh38)

Linked Dataset: Mouse genes (GRCm39)

Supporting: MyGene.info service for gene ID conversion

Required Packages:

pybiomart

pandas

mygene

Input Genes (Human GRCh38):

VEPH1 (ventral anterior homeobox 1)

UGDH (UDP-glucose 6-dehydrogenase)

FRAT2 (frequently rearranged in advanced T-cell lymphomas 2)

RNU6-686P (RNA, U6 small nuclear 686, pseudogene)

XYZ (example gene not in dataset)

Required Information to Extract:

From Human Dataset:

Human gene symbol

Human Ensembl gene ID

Human chromosome location

From Mouse Dataset:

Mouse gene symbol

Mouse Ensembl gene ID

Mouse chromosome location

Percentage identity with human ortholog

Output Format: Create a pandas DataFrame with the following columns:

Human_Gene_Symbol

Human_Ensembl_ID

Human_Chromosome

Mouse_Gene_Symbol

Mouse_Ensembl_ID

Mouse_Chromosome

Percent_Identity

Implementation Requirements:

Include error handling for genes without orthologs

Document any cases where one-to-one orthology is not found

Save results to both console output and CSV file
