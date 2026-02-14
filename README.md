# iModulonMiner 2.0

**iModulonMiner 2.0: Multi-modality modularization of prokaryotic bulk, single cell, and community omics data**

This repository contains analysis workflows and data supporting the paper.

### Packages and Workflows

- **MultiModulon package** (Python): [https://github.com/Gaoyuan-Li/multimodulon](https://github.com/Gaoyuan-Li/multimodulon)

MultiModulon documentation: [https://multimodulon.readthedocs.io/en/latest/](https://multimodulon.readthedocs.io/en/latest/)
- **MAPPED workflow** (expression data pipeline): [https://github.com/Gaoyuan-Li/MAPPED](https://github.com/Gaoyuan-Li/MAPPED)

---

Below is the project file structure (including notebooks).

---

## File structure

```
iModulonMiner_2.0/
├── 1_MultiModulon_E_coli/              # MultiModulon on E. coli strains)
│   ├── 1_Create_MultiModulon_object.ipynb
│   ├── 2_Chracterizing_Core_iModulons.ipynb
│   └── Input_Data/
│       ├── BL21/
│       │   ├── expression_matrices/
│       │   ├── ref_genome/
│       │   └── samplesheet/
│       ├── Nissle_1917/
│       │   ├── expression_matrices/
│       │   ├── ref_genome/
│       │   └── samplesheet/
│       └── O157_H7/
│           ├── expression_matrices/
│           ├── ref_genome/
│           └── samplesheet/
│
├── 2_MultiModulon_Streptomyces/       # MultiModulon on Streptomyces
│   ├── 1_Create_MultiModulon_object.ipynb
│   ├── 2_Chracterizing_Core_iModulons.ipynb
│   └── Input_Data/
│       ├── Streptomyces_albidoflavus/
│       │   ├── expression_matrices/
│       │   ├── ref_genome/
│       │   └── samplesheet/
│       └── Streptomyces_venezuelae/
│           ├── expression_matrices/
│           ├── ref_genome/
│           └── samplesheet/
│
├── 3_MultiModulon_Enterococcus/       # MultiModulon on Enterococcus
│   ├── 1_Create_MultiModulon_object.ipynb
│   ├── 2_Chracterizing_Core_iModulons.ipynb
│   └── Input_Data/
│       ├── Enterococcus_faecalis/
│       │   ├── expression_matrices/
│       │   ├── ref_genome/
│       │   └── samplesheet/
│       └── Enterococcus_faecium/
│           ├── expression_matrices/
│           ├── ref_genome/
│           └── samplesheet/
│
├── 4_MultiModulon_Multi_Modality/     # MultiModulon on proteome + transcriptome
│   ├── 1_Create_MultiModulon_object.ipynb
│   ├── 2_Chracterizing_Core_iModulons.ipynb
│   └── Data_Proteome_RNA/
│       ├── Proteomics/
│       │   ├── expression_matrices/
│       │   ├── ref_genome/
│       │   └── samplesheet/
│       └── Transcriptomics/
│           ├── expression_matrices/
│           ├── ref_genome/
│           └── samplesheet/
│
├── 5_Single_cell/                    # Single-cell 
│   ├── scanpy_CIP_iM_paperQC.ipynb
│   ├── scanpy_CIP_iM_paperQC_violin.ipynb
│   └── BBH/                         
│
├── 6_Community/                      # Community 
│   ├── 1_iM_changes_basal.ipynb
│   ├── 2_iM_PCA.ipynb
│   ├── A_Matrices/                   
│   ├── E_coli_ref_genome/
│   ├── Expression_Matrices/
│   ├── M_Matrices/                   
│   ├── P_putida_ref_genome/
│   └── X_Matrices/                  
│
├── 7_Single_View_and_Prior_Guided_Inference/
│   ├── 1_RI-ICA/                     # Robust Iterative ICA
│   │   ├── Prepare_X.ipynb
│   │   ├── Prepare_Second_X_From_run_1.ipynb
│   │   ├── Prepare_Third_X_From_run_2.ipynb
│   │   ├── Prepare_Fourth_X_From_run_3.ipynb
│   │   ├── Characterization_Run_1_to_4.ipynb
│   │   ├── First_run_100_400/
│   │   ├── Second_run_100_300/
│   │   ├── Third_run_60_180/
│   │   ├── Fourth_run_40_120/
│   │   └── P1K_minicoli_removed/
│   └── 2_SC-ALS/                     # Sparsity-Constrained ALS
│       └── Sparsity_Constrained_ALS.ipynb
│
├── 8_Activation_Confidence/          # Activation confidence
│   ├── A_confidence_P1K.ipynb
│   └── A_confidence_case_study_plotting.ipynb
│
└── 9_Basal_Expression_Transformation/
    ├── Basal_Expression_04192024.ipynb
    └── Data_Basal_Expression/        # Basal Expression Transformation
```
