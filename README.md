# 📊 Prediksi Volatilitas GOOG 2-Jam dengan Classification, Regression dan Clustering

**Tujuan**: Membangun dan membandingkan model *classification*, *regression*, serta *clustering* untuk memprediksi arah & volatilitas harga GOOG berfrekuensi menitan selama 2 jam ke depan.

## ⚙️ Cara Menjalankan
1. Unduh file `SnP_daily_update.csv` di [link ini](https://www.kaggle.com/datasets/yash16jr/s-and-p500-daily-update-dataset?select=SnP_daily_update.csv) dan letakkan di folder yang sama dengan notebook.
2. Pastikan file `Kelompok14_Data.csv` juga tersedia (diperoleh dari Alpha Vantage API atau lokal).
3. Jalankan seluruh cell notebook secara berurutan.
4. Hasil akhir:
   - **Classification**: perbandingan LSTM vs XGBoost (Confusion-Matrix & F1)
   - **Regression**: prediksi volatilitas 120-menit (LSTM vs Linear Regression)
   - **Clustering**: segmentasi pasar 15-menitan (K-Means vs GMM)

## 📌 Ringkasan Output
- *Classification*: LSTM 84 % akurasi, XGBoost 62 %
- *Regression*: LSTM R² 0,46; Linear R² -0,14
- *Clustering*: 2 klaster volatilitas (tenam vs aktif) berdasarkan Silhouette Score
