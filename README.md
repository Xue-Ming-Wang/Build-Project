# Build Project

## Project 1: 
## DNA Sequencing & Mutation Analysis with Python

This project demonstrates a bioinformatics workflow for analyzing DNA sequencing data (FASTQ format) to classify sequences, detect mutations, and assess sequencing quality. Using Biopython, sequences were grouped by index barcodes (ATGCTA and CGATAG) and compared to reference templates (template1, template2) via Hamming distance calculations to quantify mismatches (potential mutations).

Methods:
- Sequence Classification: FASTQ reads were partitioned into two groups based on index matches.
- Mutation Detection: Hamming distances identified substitutions/indels between reads and reference templates.
- Quality Control: Phred scores visualized base-call accuracy distributions per group.

Results:
- Group 1 showed higher Hamming distances (1–5 mismatches) vs. Group 2 (1–3), suggesting varied mutation rates.
- Quality histograms revealed similar Phred score distributions (peaks ~20–30), indicating consistent sequencing accuracy.
- The pipeline highlights computational tools for mutation screening and quality assessment in genomics.

## Project 2:
## Cefepime Resistance Prediction in E. coli with Machine Learning

This project aimed to predict Cefepime susceptibility (Sensitive vs. Resistant) in Escherichia coli using genomic features. Five models were trained and evaluated: Logistic Regression (LR), Random Forest (RF), Decision Tree (DT), CNN, and RNN, with stratified cross-validation (CV) and hyperparameter tuning. Feature selection was performed using L1 regularization in LR, while RF used Bayesian optimization. The CNN and RNN leveraged presence/absence gene data reshaped for deep learning.
Results:
- Logistic Regression achieved the highest balanced accuracy (87.6%) and AUC (0.928), identifying key resistance genes (e.g., *KPC-10*, *CTX-M-155*).
- CNN followed closely (85.8% accuracy), but required more computational resources.
- RF and DT performed similarly (~84%), while RNN underperformed (59.4% accuracy).
- Feature importance analysis revealed biologically plausible markers (e.g., AcrS for susceptibility).
The study highlights LR’s interpretability and performance for clinical applications, though CNN may offer incremental gains with further tuning.
