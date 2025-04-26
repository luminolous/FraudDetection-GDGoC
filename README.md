# 🛡️ Fraud Detection with Weighted Ensemble (RF + LGBM + XGB)

## 📖 Project Overview
Proyek ini bertujuan untuk membangun sistem deteksi penipuan (fraud detection) menggunakan kombinasi tiga model machine learning berbasis tree:

- Random Forest (RF)
- LightGBM (LGBM)
- XGBoost (XGB)

Akhirnya dilakukan **Weighted Ensemble** dan **Threshold Optimization** untuk meningkatkan performa prediksi.

## 🔥 Model List
- **Random Forest**: Model ensemble berbasis decision tree dengan teknik bootstrap aggregating (bagging).
- **LightGBM**: Gradient boosting framework yang cepat dan efisien.
- **XGBoost**: Model boosting yang kuat dengan regularisasi.
- **Weighted Ensemble**: Kombinasi probabilitas dari ketiga model dengan bobot:
  - RF = 20%
  - LGBM = 20%
  - XGB = 60%

## 🛠️ How to Run
1. Pastikan semua library Python berikut sudah terinstall:
   ```bash
   pip install -r requirements.txt
   ```

2. Jalankan file notebook `main.ipynb` secara berurutan.
3. Proses yang dilakukan di notebook:
   - Preprocessing data (cleaning, feature engineering)
   - Train Random Forest, LightGBM, dan XGBoost
   - Simpan hasil `predict_proba` masing-masing model
   - Buat Weighted Ensemble
   - Optimasi Threshold
   - Buat submission file untuk Kaggle

## 🔟 Final Output
- Submission file utama:
  - `final_submit_weighted_w202060_t270.csv`
  - `final_submit_weighted_w202060_t275.csv`
- Threshold terbaik digunakan adalah antara **0.270 - 0.275** berdasarkan tuning di validation set.

## 🔹 Highlights
- Threshold tuning meningkatkan Precision & Recall seimbang.
- Bobot lebih besar pada XGB memberikan hasil lebih stabil.

---

> ⭐️ If you find this useful, please star the repo!

