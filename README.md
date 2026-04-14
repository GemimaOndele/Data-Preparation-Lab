# Data Preparation Lab

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

End-to-end data preparation workflow with robust cleaning, exploratory visual diagnostics, and publication-ready KPI dashboards.

This repository contains my **Data Preparation Lab** for the *Introduction to Computer Vision* course.

## Contents

- `Data_Preparation_Lab.ipynb`: full notebook (data loading, cleaning, visual analysis, 3D plots, and KPI dashboard export).
- `linkedin_export/`: generated publication assets (charts, dashboard image, captions, and LinkedIn post template).
- `BookDataCleaning.pdf`: course support material used for the lab.
- `Dataset/cleaned_individual/`: one cleaned output per source file, each saved as an individual compressed `.csv.gz`.
- `Dataset/cleaned_individual_bundle.zip`: ZIP archive containing all individually compressed cleaned outputs.

## Dataset

The lab is based on the Kaggle missing-values practice dataset:

<https://www.kaggle.com/code/alexisbcook/handling-missing-values>

Raw CSV files are not tracked in this repo because they are large.

## Reproducibility

1. Download the dataset files and place them in `Dataset/`.
2. Open `Data_Preparation_Lab.ipynb`.
3. Run all notebook cells in order.
4. Run the export section to regenerate:
   - cleaned individual files in `Dataset/cleaned_individual/`,
   - the ZIP bundle `Dataset/cleaned_individual_bundle.zip`,
   - publication assets in `linkedin_export/`.

## Output Format

| Path | Role | Format |
|---|---|---|
| `Dataset/cleaned_individual/` | Stores one cleaned result per raw CSV source file | `.csv.gz` (individually compressed) |
| `Dataset/cleaned_individual_bundle.zip` | Single archive that groups all cleaned individual outputs | `.zip` |
| `linkedin_export/` | Publication-ready visuals and text assets | `.png`, `.md` |
| `Data_Preparation_Lab.ipynb` | Main end-to-end workflow (cleaning, EDA, dashboard generation) | Jupyter Notebook |

## Quick Start (Conda)

```bash
conda create -n data-prep-lab python=3.11 -y
conda activate data-prep-lab
conda install pandas numpy matplotlib seaborn jupyter -y
jupyter notebook
# then open and run Data_Preparation_Lab.ipynb (Run All)
```

Alternative without Conda:

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook
```

## Author

Gemima ONDELE — MSc 1 AI
