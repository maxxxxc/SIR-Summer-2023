# Binary Classification by Divide and Conquer Approach

This repository contains the code and supporting materials for a research project focused on exploring use cases of **binary classification** through a **divide-and-conquer** approach.

> 📰 **Published in ICMI 2025 Proceedings**  
> IEEE link: [https://ieeexplore.ieee.org/document/10586091](https://ieeexplore.ieee.org/document/10586091)

## 🔍 Project Overview

This project explores the **divide and conquer approach** for implementing **distributed logistic regression** and **support vector machine (SVM)** algorithms in the context of large-scale binary classification tasks. In our approach:

1. The dataset is **partitioned** across multiple processors or nodes.
2. Each subset is processed independently using either **logistic regression** or **SVM**, producing local classifiers.
3. These local models are then **aggregated** to form a **global classifier** capable of making final predictions.

We investigate three aggregation strategies:
- **Voting** based on predicted class labels,
- **Averaging** of raw real-valued predictions,
- **Averaging of posterior probabilities**.

**Key Findings**:
- For distributed **logistic regression**, **posterior probability averaging** offers the most robust performance and is the recommended approach.
- For distributed **SVM**, posterior probability averaging adds modeling complexity without significant gains. Thus, **functional (real-valued) averaging** is preferred.

## 📂 Repository Contents

- `dataset/` — Containts all input datasets. 
- `Main Scripts/` — Analysis code for all datasets (includes Logistic Regression and SVMs)
- `Output Results/` — Output results for all datasets 
- `Jupyter Notebook Code/` — All other miscellaneous code, mostly comprised of individual dataset analysis code. 


