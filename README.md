# 20.440 Project – Reproducing Heatmap from CellPhoneDB Results

## Overview
This repository contains code and data needed to reproduce a heatmap figure from my 20.440 project. The heatmap shows statistically significant ligand–receptor interactions within cardiomyocyte (CM) monoculture, inferred using CellPhoneDB.

## Data
The dataset used here was generated using CellPhoneDB with input from a single-cell RNA-seq dataset of iPSC-derived cardiomyocytes. For replicating the heatmap of signficant interactions between cells in the CM Monoculture the only file needed is CellphoneDB_Results/CM/statistical_analysis_pvalues_04_07_2025_191005.txt.

## Folder Structure
- `code/`: contains the notebook used to generate the figure
- `CellphoneDB_Results/`: contains the CellPhoneDB result files for both the CM monoculture and CM-EC coculture
- `.gitignore`, `.gitattributes`: Git configuration files

## Installation
1. Create and activate new environment
conda create -n cpdb-heatmap python=3.10
conda activate cpdb-heatmap

2. Install dependencies
pip install pandas ktplotspy

## Citation
Troulé K, Petryszak R, Cakir B, Cranley J, Harasty A, Prete M, Tuong ZK, Teichmann SA, Garcia-Alonso L, Vento-Tormo R. 2025. CellPhoneDB v5: inferring cell–cell communication from single-cell multiomics data., Nature Protocols. doi:10.1038/s41596-024-01137-1.
