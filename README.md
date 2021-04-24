# PSSM_Files_of_ALL_SwissProt_Proteins
 This repository contains the [link](https://drive.google.com/drive/folders/1XYZG8NIVMjTb1eBoF54KCByLCv6IZcSQ?usp=sharing) for all Position-Specific Scoring Matrices(PSSMs) of all protein in SwissProt(UniProtKB).
 
 These PSSMs are created by using **PSI BLAST** and [UniRef50](https://www.uniprot.org/uniref/?query=&fil=identity:0.5) database from [UniProtKB](https://www.uniprot.org/).
## What is a PSSM?
A PSSM, or Position-Specific Scoring Matrix, is a type of scoring matrix used in protein BLAST searches in which amino acid substitution scores are given separately for each position in a protein multiple sequence alignment. Thus, a Tyr-Trp substitution at position A of an alignment may receive a very different score than the same substitution at position B. This is in contrast to position-independent matrices such as the PAM and BLOSUM matrices, in which the Tyr-Trp substitution receives the same score no matter at what position it occurs.

PSSM scores are generally shown as positive or negative integers. Positive scores indicate that the given amino acid substitution occurs more frequently in the alignment than expected by chance, while negative scores indicate that the substitution occurs less frequently than expected. Large positive scores often indicate critical functional residues, which may be active site residues or residues required for other intermolecular interactions.

PSSMs can be created using PSI-BLAST, which finds similar protein sequences to a query sequence, and then constructs a PSSM from the resulting alignment. Alternatively, PSSMs can be retrieved from the NCBI CDD database, since each CD is represented by a PSSM that encodes the observed substitutions in the seed alignments. These CD records can be found either by text searching in Entrez Conserved Domains or by using RPS-BLAST (Reverse Position-Specific BLAST), also known as CD-Search, to locate these domains on an input protein sequence.

This information is taken from [here].(https://www.ncbi.nlm.nih.gov/Class/Structure/pssm/pssm_viewer.cgi#:~:text=A%20PSSM%2C%20or%20Position%2DSpecific,a%20protein%20multiple%20sequence%20alignment)

The following is a screenshot of a sample PSSM.

![alt text](https://github.com/gozsari/PSSM_Files_of_ALL_SwissProt/blob/main/images/pssm.PNG)
## What is PSI BLAST?
PSI-BLAST (Position-Specific Iterative Basic Local Alignment Search Tool) derives a position-specific scoring matrix (PSSM) or profile from the multiple sequence alignment of sequences detected above a given score threshold using protein–protein BLAST. This PSSM is used to further search the database for new matches, and is updated for subsequent iterations with these newly detected sequences. Thus, PSI-BLAST provides a means of detecting distant relationships between proteins. In this chapter, we discuss practical aspects of using PSI-BLAST and provide a tutorial on how to uncover distant relationships between proteins and use them to reach biologically meaningful conclusions.

This information is taken from [here].(https://www.ncbi.nlm.nih.gov/books/NBK2590/#:~:text=Summary,threshold%20using%20protein%E2%80%93protein%20BLAST.)

![alt text](https://github.com/gozsari/PSSM_Files_of_ALL_SwissProt/blob/main/images/psi_blast.png)