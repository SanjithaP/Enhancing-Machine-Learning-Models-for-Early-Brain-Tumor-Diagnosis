#  Machine Learning for Brain Tumor Classification

Early diagnosis system for brain tumors using plasma metabolomics and machine learning algorithms.

## Overview

This project develops a machine learning-based diagnostic system to classify brain tumors (glioma and meningioma) by analyzing 188 metabolites from plasma samples. The system achieves up to 98.5% accuracy using the EvoHDTree algorithm with ADASYN upsampling.

**Author:** Sanjitha P | **Guide:** Dr. Brindha GR | **Institution:** SASTRA University | **Year:** 2023

## Key Features

- **10 ML Models**: Comparison of NB, GLM, LR, FLM, DL, DT, RF, GBT, SVM, and EvoHDTree
- **Grade-Specific Classification**: Distinguishes glioma grades (I-IV) from healthy controls
- **Class Imbalance Handling**: ADASYN upsampling for improved performance
- **Interactive GUI**: Streamlit-based web interface for predictions

## Results

| Classification Task | Accuracy | AUC | F1-Score |
|---------------------|----------|-----|----------|
| Glioma Grade IV vs Control | 98.5% | 0.971 | 0.985 |
| Glioma (I-IV) vs Control | 95.2% | 0.951 | 0.958 |
| Meningioma vs Control | 87.8% | 0.840 | 0.857 |

**Best Model:** EvoHDTree (Evolutionary Heterogeneous Decision Tree)

## Dataset

- **Source:** Plasma metabolomics data (41598_2023_38243_MOESM2_ESM.xlsr)
- **Samples:** 95 glioma + 70 meningioma + 71 healthy controls
- **Features:** 188 metabolites per sample

## Technical Highlights

- **Novel Contribution:** EvoHDTree implementation with ADASYN upsampling
- **Validation:** Leave-One-Out Cross-Validation
- **Metrics:** Accuracy, AUC-ROC, F1-score
- **Visualization:** ROC curves, confusion matrices, class distribution plots

## Future Work

- Integration with larger multi-center datasets
- Mobile application deployment
- Real-time prediction capabilities
- Fusion with medical imaging data

## License

BSD-3-Clause License - see [LICENSE](LICENSE) file


## Reference Paper

Godlewski, A., et al. (2023). "A comparison of different machine-learning techniques for the selection of a panel of metabolites allowing early detection of brain tumors." *Scientific Reports*, 13, 11044. [DOI: 10.1038/s41598-023-38243-1](https://doi.org/10.1038/s41598-023-38243-1)

---

⚠️ **Note:** This is a research prototype. Clinical validation required before deployment.
