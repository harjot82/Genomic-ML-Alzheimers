# Genomic-ML-Alzheimers

Machine learning–based genomic risk stratification for Alzheimer’s disease using an interpretable multi-class classification framework.

---

## 🧠 Project Overview

Alzheimer’s disease is a complex and heterogeneous neurodegenerative disorder with strong genetic underpinnings. While machine learning methods have shown promise in disease prediction, many approaches lack interpretability, limiting their usefulness for biological understanding and downstream research.

In this project, **I explore an interpretable machine learning framework for genomic risk stratification in Alzheimer’s disease**, developed using a **curated genomic dataset provided as part of a hackathon challenge**. The focus of this work is not only on predictive performance, but also on **model transparency, confidence estimation, and human-interpretable decision support**.

---

## 🎯 Objectives

The primary objectives of this work are to:

- Perform multi-class classification using genomic feature representations  
- Emphasize interpretability of model decisions using feature importance and SHAP  
- Introduce confidence-based risk stratification as an application layer  
- Provide a reproducible and educational framework for genomic machine learning analysis  

---

## ⚙️ Methodology

**Input Data**
- Preprocessed, high-dimensional genomic feature representations  
- Dataset provided as part of the hackathon challenge

**Model**
- Random Forest multi-class classifier

**Preprocessing**
- Log transformation and clipping to control extreme genomic values  
- Conversion to numerical formats compatible with classical ML models

**Evaluation**
- Classification accuracy  
- Confusion matrix analysis  
- Prediction confidence score distribution  

**Interpretability**
- Random Forest feature importance  
- SHAP (SHapley Additive exPlanations)–based feature contribution analysis  

---

## 🧩 Model Selection Rationale

I selected a **Random Forest classifier** due to its ability to handle high-dimensional tabular genomic data, capture non-linear feature interactions, and provide built-in measures of feature importance.

Tree-based ensemble models offer a practical balance between **predictive power and interpretability**, making them well-suited for exploratory genomic analysis under hackathon constraints. This choice also enables confidence-based risk stratification and transparent feature relevance analysis.

---

## 🔍 Interpretability & Risk Stratification

Model interpretability is a central component of this project. Feature relevance was examined using both Random Forest feature importance and SHAP-based explanations, providing insight into which genomic features most strongly influence model predictions.

In addition, I analyzed **prediction confidence scores** and used them to stratify samples into:
- **High-priority cases** (high-confidence predictions)  
- **Lower-priority cases** (ambiguous or overlapping genomic signatures)

This confidence-based stratification serves as a human-interpretable layer that may support downstream validation or prioritization workflows.

---

## 📊 Key Observations

- The model achieved near-perfect performance on the provided dataset, indicating strong separability within the curated genomic feature space.  
- Confidence score distributions revealed a small subset of lower-confidence predictions, consistent with known genetic heterogeneity in Alzheimer’s disease.  
- Interpretability analyses showed consistent feature relevance across methods.

> **Note:** Such performance may not directly generalize to real-world clinical cohorts and requires external validation.

---

## ⚠️ Limitations

- The model is trained on a curated, hackathon-provided dataset  
- No independent external cohort validation was performed  
- Results should be interpreted as exploratory rather than clinically actionable  

---

## 🚀 Future Work

Future extensions of this work may include:
- Validation on independent or longitudinal genomic cohorts  
- Integration with molecular docking or in vitro experimental pipelines  
- Extension to multi-omics or pathway-level feature representations  

---

## 👩‍💻 Author

Harjot Kaur  
LinkedIn: https://www.linkedin.com/in/harjot-k-ba497b209
