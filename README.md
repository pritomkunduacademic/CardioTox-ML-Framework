# 🧬 Precision Cardiotoxicity Prediction: A Stacked Machine Learning Framework for hERG Inhibition

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-FFB000?style=for-the-badge&logo=lightgbm&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-FF6F00?style=for-the-badge&logo=machine-learning&logoColor=white)
![ChEMBL](https://img.shields.io/badge/Data-ChEMBL%20Database-00517C?style=for-the-badge)
![Target](https://img.shields.io/badge/Target-hERG%20Symbol-E91E63?style=for-the-badge)

## 🏛️ Academic Reflection
*Research Statement for MRes/PhD Candidacy*

In the lifecycle of drug discovery, unintended inhibition of the **hERG (human Ether-à-go-go-Related Gene)** potassium channel represents a major regulatory bottleneck. Such inhibition can lead to QT interval prolongation and fatal cardiac arrhythmias. This project addresses the **"Shift-Left" paradigm** in pharmaceutical research—integrating safety assessment into the earliest stages of lead optimization using high-fidelity computational modeling.

This work demonstrates my ability to navigate the complexities of chemical informatics and ensemble learning. By implementing a **Stacked Generalization Framework**, I showcase a sophisticated understanding of how to mitigate the variance and bias inherent in biological data. This project serves as a testament to my technical readiness for advanced graduate research in **Bioinformatics and Cheminformatics**.

---

## 🚀 Key Research Features
* **📡 Automated Bioactivity Pipeline:** Direct API integration with **ChEMBL (Target ID: ChEMBL240)** for real-time data retrieval and curation.
* **🏗️ Hierarchical Stacking Architecture:** A multi-layered ensemble approach combining **LightGBM**, **XGBoost**, and **Random Forest** to achieve superior predictive stability.
* **🧬 Molecular Representation:** Advanced featurization using **Morgan Fingerprints (Radius 2, 2048-bit)** to capture local chemical environments and pharmacophoric patterns.
* **⚖️ Imbalance Calibration:** Strategic use of class-weight adjustments to ensure high sensitivity in detecting cardiotoxicants.
* **📊 Publication-Grade Analytics:** Automated generation of 600 DPI visualizations, including **ROC-AUC curves**, **Precision-Recall plots**, and feature importance maps.

---

## 🛠️ Tech Stack & Methodology
### **Environment & Tools**
* **Google Colab:** Cloud-based environment for high-performance model training.
* **Python 3.10+:** Core programming language.

### **Computational Chemistry & ML**
* **RDKit:** Chemical standardization, SMILES canonicalization, and descriptor generation.
* **Scikit-Learn:** Implementation of the `StackingCVClassifier` and rigorous cross-validation pipelines.
* **LightGBM & XGBoost:** High-efficiency gradient boosting frameworks optimized for leaf-wise growth.
* **Pandas & NumPy:** For complex data engineering and matrix operations.

---

## 📋 Scientific Workflow
1.  **Data Acquisition:** Automated extraction of hERG bioactivity assays (IC50/pChEMBL values).
2.  **Chemical Engineering:** Conversion of SMILES strings into numerical vectors using Circular Fingerprints.
3.  **Ensemble Training:** Base models are trained in parallel to capture diverse structural alerts.
4.  **Stacked Generalization:** A Meta-Learner (Logistic Regression/SVM) aggregates base-model outputs to produce a final, high-confidence toxicity prediction.
5.  **Statistical Validation:** Rigorous evaluation focused on **Matthews Correlation Coefficient (MCC)** to ensure the model's robustness against imbalanced datasets.

---

## 📂 Project Structure
```text
├── MLToxicological_Modeling_hERG.ipynb   # Full Research & Stacking Pipeline
├── image_a755b6.png                      # Statistical Visualization Results
├── 01_Data/
│   └── hERG_bioactivity_raw.csv          # Raw data curated from ChEMBL240
├── 02_Output/
│   ├── ML_Ready_Dataset.xlsx             # Feature-engineered matrix
│   └── Serialized_Stacking_Model.pkl     # Final Meta-Model for inference
