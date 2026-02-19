# 🧠 Harmonised MCI-SSL  
Early Detection and Classification of Alzheimer’s Disease using Multimodal Learning & Domain Harmonisation  

---

## 📌 Overview

Harmonised MCI-SSL is a conference-accepted research project focused on improving the early detection of Alzheimer’s Disease (AD) using MRI data.

The framework integrates:

- 3D CNN-based MRI feature extraction  
- Self-Supervised Learning (Denoising Autoencoder)  
- Multimodal fusion of imaging, clinical, and genetic biomarkers  
- Domain harmonisation for cross-site robustness  
- Hybrid CNN-SVM classification  

This work specifically investigates the impact of scanner-induced domain shift and proposes harmonisation strategies to improve generalisation across imaging sites.

---

## 🎯 Key Contributions

- ✅ Unified pipeline integrating SSL + Multimodal Learning + Harmonisation  
- ✅ Quantitative measurement of domain shift impact  
- ✅ Demonstrated cross-site performance improvement (+31.62%)  
- ✅ High within-site test accuracy (99.58%)  
- ✅ Fast inference (< 1 second per scan)

---

## 📊 Dataset

- OASIS MRI Dataset  
- 9,489 T1-weighted structural MRI scans  
- Stratified 80/20 train-test split  
- Alzheimer’s Disease cases: 5.2% (class imbalance handled via model design)

---

## 🧪 Methodology

1. **MRI Feature Extraction**  
   Pretrained 3D ResNet-18 model used to extract 512-dimensional features.

2. **Self-Supervised Learning (SSL)**  
   Denoising autoencoder reduces feature dimensionality to 128 while improving robustness.

3. **Multimodal Fusion**  
   Integration of:
   - MRI features  
   - Clinical biomarkers (MMSE, CDR)  
   - Genetic marker (APOE ε4)

4. **Domain Harmonisation**  
   Site-wise standardisation applied to mitigate scanner-induced domain shift.

5. **Classification**  
   Support Vector Machine (RBF kernel) for final prediction.

---

## 📈 Performance Summary

- Test Accuracy: 99.58%  
- Sensitivity (AD): 98.98%  
- Specificity (CN): 99.83%  
- Misclassifications: 7 / 1,898  
- 5-Fold Cross-Validation: 88.50% ± 3.16%  
- Cross-site accuracy improvement after harmonisation: +31.62%

---

## 📂 Repository Contents

- `HHARMONIZEDMCI_SSL.ipynb` → Complete experimental pipeline  

---

## 📄 Publication Status

This work has been accepted for presentation at ICASS 2026.

The repository contains the implementation of the proposed methodology.  
The final published version will appear in the official conference proceedings.

---

## 🔮 Future Work

- Validation on real multi-site datasets (e.g., ADNI)  
- Longitudinal disease progression modelling  
- Integration of Explainable AI (SHAP / Grad-CAM)  
- Real-world clinical deployment studies  

---

## 👩‍💻 Author

**Pari Bansal**  
B.Tech CSE (AI & ML)  
K.R. Mangalam University  
Conference Presenter – ICASS 2026  

---

## ⚖️ License

This project is licensed under the MIT License.
