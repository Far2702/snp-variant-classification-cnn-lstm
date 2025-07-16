# **Variant Classification of SNPs using a custom CNN-LSTM dual input architecture**

# Introduction
Single Nucleotide Polymorphisms (SNPs) are the most common type of genetic variation among individuals and play a crucial role in disease susceptibility, drug response, and personalized medicine. Accurate classification of SNPs as benign or pathogenic is essential for genomic diagnostics and therapeutic decision-making. Traditional approaches often rely on handcrafted features and statistical models, which may not fully capture the underlying sequence context and biological patterns.

In this project, I have made a custom deep learning architecture that combines Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTM) networks to classify SNP variants. By leveraging dual input channels—one for reference sequences and another for alternate sequences—we aim to extract both local sequence motifs and long-range dependencies.

# Dataset
The dataset used for this project was obtained from **ClinVar**, a publicly available resource maintained by the **National Center for Biotechnology Information (NCBI)**. ClinVar aggregates information about genomic variations and their relationship to human health, including clinical significance annotations such as pathogenic, benign, likely pathogenic, and uncertain significance.

For this project, only **Single Nucleotide Polymorphisms (SNPs)** with clearly defined clinical labels (pathogenic and benign) were selected to ensure binary classification. Each variant entry includes the reference and alternate alleles along with the surrounding genomic sequence, which were used to construct the input features for the model.I have taken the Reference Sequences from the **Ensembl API**.

# Model
I have read a [Research Paper](https://pmc.ncbi.nlm.nih.gov/articles/PMC8285202/#B6) with the title of **Analysis of DNA Sequence Classification Using CNN and Hybrid Models**.
I have read the resrach paper where they compared different CNN moeels for accuracy in classification tasks. 

After reading this I have come up with a new architecture of dual input CNN-LSTM structure to classify the DNA sequences.
The



