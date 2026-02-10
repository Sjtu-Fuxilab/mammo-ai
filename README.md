# Cross-Paradigm Transfer in Mammography AI

"Cross-Paradigm Transfer in Mammography AI: A Multi-Domain Evaluation of Performance, Fairness Gaps, and Uncertainty-Stratified Effects"

Authors: Sanwal Ahmad Zafar, Wei Qin (corresponding), Liu Chengliang, Areeba Ali Khan, Muhammad Salman Faisal  
Corresponding author: Wei Qin (wqin@sjtu.edu.cn)

## Code
This repository contains the full pipeline (data handling hooks, training, evaluation, and reproduction of paper figures/tables).

## Datasets
This work uses third-party datasets available from their original providers under their respective licenses and access requirements:

- RSNA Breast Cancer Detection (Kaggle): https://www.kaggle.com/c/rsna-breast-cancer-detection
- CMMD (TCIA): https://www.cancerimagingarchive.net/collection/cmmd/
- VinDr-Mammo (PhysioNet; restricted access / DUA): https://physionet.org/content/vindr-mammo/
- INbreast (originating provider; some mirrors exist): https://www.kaggle.com/datasets/itiresearch/inbreastdensetissue
- NLBS / NL-Breast-Screening (FRDR): https://www.frdr-dfdr.ca/repo/dataset/cb5ddb98-ccdf-455c-886c-c9750a8c34c2

Notes:
- Outcome model is trained on pathology-confirmed outcomes (RSNA + CMMD).
- Assessment model is trained on BI-RADS–based labels (VinDr).
- INbreast and NLBS are used as external evaluation datasets (NLBS includes a recall/no-recall subset for evaluation).

## Reproducibility
- Notebook: `ct.ipynb`
- We do not redistribute any dataset files. Users must obtain datasets directly from the sources above.
- Before running, set your local data paths in the notebook configuration cell.

Last updated: 2026-01-08
