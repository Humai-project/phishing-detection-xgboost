# Phishing Website Detection using XGBoost + GridSearchCV

Replication study dari penelitian Shaukat et al. (2023) dengan kontribusi 
penerapan hyperparameter tuning berbasis GridSearchCV pada algoritma XGBoost.

## Deskripsi
Penelitian ini mendeteksi website phishing menggunakan machine learning 
dengan tiga model: Decision Tree, Random Forest, dan XGBoost yang dioptimalkan 
menggunakan GridSearchCV.

## Hasil Eksperimen
| Model | Accuracy | Recall | F1-Score | AUC-ROC |
|-------|----------|--------|----------|---------|
| Decision Tree | 93.09% | 93.18% | 93.09% | 0.9309 |
| Random Forest (Baseline) | 96.19% | 96.68% | 96.21% | 0.9924 |
| XGBoost + GridSearchCV (Usulan) | **96.46%** | **97.29%** | **96.49%** | **0.9925** |

## Dataset
- **Nama:** Phishing Dataset for Machine Learning
- **Sumber:** [Kaggle](https://www.kaggle.com/datasets/shashwatwork/web-page-phishing-detection-dataset)
- **Jumlah data:** 11.430 sampel
- **Jumlah fitur:** 87 fitur numerik
- **Distribusi kelas:** Seimbang (5.715 legitimate : 5.715 phishing)

## Cara Menjalankan
1. Buka Google Colab: [colab.research.google.com](https://colab.research.google.com)
2. Upload file `phishing_detection_colab.ipynb`
3. Upload file `dataset_phishing.csv`
4. Klik **Runtime → Run All**
5. Tunggu sekitar 5-10 menit sampai semua cell selesai

## Library yang Digunakan
pandas

numpy

matplotlib

seaborn

scikit-learn

xgboost

joblib

## Struktur File
├── phishing_detection_colab.ipynb  # Notebook utama

├── dataset_phishing.csv            # Dataset

├── hasil_evaluasi_lengkap.png      # Grafik hasil evaluasi

├── eda_distribusi.png              # Grafik distribusi dataset

├── xgboost_phishing_model.pkl      # Model XGBoost tersimpan

├── randomforest_baseline.pkl       # Model Random Forest tersimpan

└── README.md                       # Dokumentasi ini

## Paper Acuan
Shaukat, M.W., Amin, R., Muslam, M.M.A., Alshehri, A.H., & Xie, J. (2023). 
A Hybrid Approach for Alluring Ads Phishing Attack Detection Using Machine Learning. 
*Sensors*, 23(19), 8070. https://doi.org/10.3390/s23198070
