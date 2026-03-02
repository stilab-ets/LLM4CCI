# Unveiling the Performance of Large Language Models for Code Change Intent Prediction Using Instance Space Analysis (LLM4CCI): Replication Package

This repository provides the complete replication package for our study on the performance of Large Language Models (LLMs) in **code change intent prediction**. It contains the datasets, scripts, and results required to reproduce our analysis.

---

## 📂 Repository Structure

### Data Collection
The datasets are available in the [data](data/) folder. They include CSV files for the **Android**, **OpenStack**, and **Qt** projects.  
Data was collected and preprocessed using the scripts provided in the [Scripts](Scripts/) directory.

### Key Scripts
- **[PyDriller](https://github.com/ishepard/pydriller)** – A Python framework for mining Git repositories. It enables extraction of commits, developers, modified files, diffs, and source code.  
- **[LLM4CCI.py](Scripts/LLM4CCI.py)** – Main script for processing and analyzing code changes using LLMs.  
- **[get_features.ipynb](Scripts/get_features.ipynb)** – Extracts features from commit data.  
- **[get_diff.ipynb](Scripts/get_diff.ipynb)** – Extracts code diffs.  
- **[BinaryRelevance.ipynb](Scripts/BinaryRelevance.ipynb) / [ClassifierChain.ipynb](Scripts/ClassifierChain.ipynb)** – Multi-label classification analysis pipelines.  
- **[bert.ipynb](Scripts/bert.ipynb) / [roberta.ipynb](Scripts/roberta.ipynb)** – Embedding generation and classification using transformer models.  
- **[ISA](Scripts/ISA/)** – MATLAB scripts for instance space analysis and visualization.  

### Statistical Analysis
Replication of statistical analyses can be found in the [Scripts](Scripts/) directory. These scripts reproduce the quantitative evaluation performed in the paper.

---

## 📊 Results and Plots
All processed results and plots are organized under the [Results](Results/) directory:

- **[RQ1](Results/RQ1/)** – Processed CSV results for each project (Gemini vs. Heuristics).  
- **[RQ2](Results/RQ2/)** – Comparative results across all studied LLMs.  
- **[RQ3](Results/RQ3/)** – Distribution plots and feature analysis.  
- **[RQ4](Results/RQ4/)** – Instance space analysis footprints, highlighting the strengths and weaknesses of each model.  

---
