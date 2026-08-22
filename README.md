<div align="center">

# 🌾 Plant-MultiOmics-Framework

**Integrative Multi-Omics Data Analysis Pipeline: Ionomics, RNA-seq Transcriptomics, Metabolomics & Statistical Network Biology for Plant Abiotic Stress**

[![R >= 4.2](https://img.shields.io/badge/R-%3E%3D%204.2-276DC3.svg?logo=r&logoColor=white)](https://www.r-project.org/)
[![Multi-Omics](https://img.shields.io/badge/Omics-Ionomics_%7C_RNAseq_%7C_Metabolomics-ff6b6b.svg)](https://github.com/PALP31/Plant-MultiOmics-Framework)
[![mixOmics](https://img.shields.io/badge/Integration-mixOmics_DIABLO-00e5bc.svg)](http://mixomics.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)

</div>

---

## 📖 Overview

**Plant-MultiOmics-Framework** is an open-source analytical framework designed to process, model, and integrate heterogeneous high-dimensional biological data across three primary regulatory layers (**Ionomics**, **Transcriptomics**, and **Metabolomics**) to uncover systems-level mechanisms of plant stress tolerance (such as terminal heat and drought in *Triticum durum* and other crops).

```
┌─────────────────┐      ┌─────────────────┐      ┌─────────────────┐
│   IONÓMICA ⚡   │      │ TRANSCRIPTOMA 🧬│      │  METABOLOMA 🧪  │
│  ICP-OES (K+/Na+)│      │ RNA-seq/DESeq2  │      │  Osmolitos/ROS  │
└────────┬────────┘      └────────┬────────┘      └────────┬────────┘
         │                        │                        │
         └─────────────────► sPLS-DA (DIABLO) ◄────────────┘
                                  │
                                  ▼
                   Piecewise SEM & Causal Networks 🕸️
```

---

## 🔬 Multi-Omics Layers & Pipelines

### 1. ⚡ Ionomics & Elemental Balance
* Quantitative ICP-OES/MS elemental profile processing.
* Ion transport balance: $K^+/Na^+$ selectivity index, vacuolar sequestration metrics, and micronutrient ratios ($Fe, Zn, Mn, Ca, Mg$).

### 2. 🧬 RNA-seq Transcriptomics & Gene Networks
* Differential gene expression workflows using `DESeq2` and `edgeR`.
* Weighted Gene Co-expression Network Analysis (`WGCNA`) for module-trait associations.
* Functional enrichment analysis (GO, KEGG, MapMan) for heat shock factors (HSFs), chaperones (HSPs), and stress-responsive regulons.

### 3. 🧪 Metabolomics & Antioxidant Phenotyping
* Quantitative profiling of compatible solutes (proline, soluble sugars, glycine betaine).
* Enzymatic antioxidant defense kinetics (SOD, CAT, APX, GR) and oxidative damage markers (MDA lipid peroxidation, $H_2O_2$).

### 4. 📊 Multi-Block Data Integration & Piecewise SEM
* Multi-block sparse Partial Least Squares Discriminant Analysis (**sPLS-DA / DIABLO**) via `mixOmics`.
* Structural Equation Modeling (**Piecewise SEM**) linking transcriptomic modules, ionic flux, and metabolic outputs directly to final yield and physiological fitness.

---

## 🛠️ Tech Stack

* **Bioinformatics**: `Bioconductor` • `DESeq2` • `WGCNA` • `mixOmics` • `clusterProfiler`
* **Modeling & Bioestadística**: `easyModels` • `piecewiseSEM` • `brms` • `lme4`
* **Visualization**: `pheatmap` • `ComplexHeatmap` • `ggplot2` • `Quarto`

---

<div align="center">
  <sub>Developed by <strong>Paúl Alexander López Peña</strong> • Pontificia Universidad Católica de Chile (PUC)</sub>
</div>
