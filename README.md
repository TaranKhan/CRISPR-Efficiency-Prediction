# 🧬 CRISPR Efficiency Prediction  
**Predicting guide RNA activity using sequence features and machine learning**

---

## 📖 Overview
This project explores how biological sequence features can influence **CRISPR-Cas9 gene-editing efficiency**.  
Using Python and machine learning, I built a simple model that learns patterns between guide RNA (gRNA) composition and its predicted editing success rate.

The dataset here is synthetic, but the workflow reflects a realistic **bioinformatics analysis pipeline** — from feature engineering to model evaluation and visualization.

---

## ⚗️ Project Highlights
- 🔡 **Sequence-based feature extraction** — GC content, nucleotide counts, melting temperature  
- 🎯 **Modeling** — Gradient Boosting Regressor to estimate CRISPR efficiency  
- 📊 **Evaluation metrics** — R², Mean Squared Error, and Spearman correlation  
- 🧠 **Visual insights** — feature importance ranking, predicted vs actual plot, and correlation matrix  

---

## 🧪 Methods and Workflow
1. **Data Simulation:**  
   Generated synthetic 20-nt gRNA sequences with random biological and experimental attributes.  
2. **Feature Engineering:**  
   Extracted sequence-level descriptors (A/T/G/C content, GC%, Tm, PAM distance, and off-target mismatches).  
3. **Model Training:**  
   Trained a `GradientBoostingRegressor` to predict numeric efficiency scores.  
4. **Validation:**  
   Used train-test split and 5-fold cross-validation to assess model robustness.  
5. **Visualization:**  
   Produced interpretable charts to understand model behavior and feature influence.

---

## 🧰 Tools & Libraries
| Category | Tools Used |
|-----------|-------------|
| Programming | Python 3 |
| ML / Stats | scikit-learn, SciPy |
| Data Processing | pandas, numpy |
| Bioinformatics | Biopython |
| Visualization | matplotlib, seaborn |

---

## 📊 Example Output
The model identifies GC content and melting temperature as key predictors.  
Although trained on synthetic data, the pipeline structure can be extended to real CRISPR datasets (e.g., Doench et al. 2016).

*(Example visualizations include feature importance barplots and correlation heatmaps.)*

---

## 🚀 How to Run Locally
```bash
# Clone the repository
git clone https://github.com/TaranKhan/CRISPR-Efficiency-Prediction.git

# Move into the project directory
cd CRISPR-Efficiency-Prediction

# Launch Jupyter Notebook
jupyter notebook
