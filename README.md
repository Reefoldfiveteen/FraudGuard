# FraudGuard: Hybrid Machine Learning Approach for Transaction Security

[![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.7.0-orange)](https://scikit-learn.org/)

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk mendeteksi potensi penipuan (*fraud*) pada transaksi perbankan dengan mengintegrasikan dua pendekatan Machine Learning:
1. **Unsupervised Learning (Clustering):** Mengelompokkan data transaksi tanpa label menggunakan algoritma K-Means untuk mengidentifikasi pola perilaku.
2. **Supervised Learning (Klasifikasi):** Membangun model Decision Tree untuk memprediksi kategori transaksi berdasarkan label yang dihasilkan dari tahap clustering.

## 🛠️ Tech Stack & Library
* **Python** sebagai bahasa pemrograman utama.
* **Pandas & NumPy** untuk manipulasi data.
* **Matplotlib & Seaborn** untuk visualisasi data (EDA).
* **Scikit-Learn (v1.7.0)** untuk pemodelan Machine Learning (PCA, KMeans, Decision Tree).
* **Yellowbrick** untuk visualisasi Elbow Method.
* **Joblib** untuk penyimpanan model (.h5).

## 🚀 Alur Kerja Proyek
1. **Exploratory Data Analysis (EDA):** Analisis korelasi dan distribusi fitur transaksi.
2. **Preprocessing:** * Pembersihan data (Handling Null & Duplicates).
   * Feature Engineering (Binning pada nominal transaksi).
   * Scaling menggunakan `StandardScaler`.
3. **Clustering:** * Reduksi dimensi menggunakan **PCA**.
   * Penentuan K-optimal dengan **Elbow Method**.
   * Segmentasi data menjadi 4 cluster utama.
4. **Classification:**
   * Pembagian data (Train-Test Split).
   * Pembangunan model **Decision Tree**.
   * **Hyperparameter Tuning** menggunakan GridSearchCV untuk akurasi optimal.

## 📊 Hasil Analisis
* **Cluster Optimal:** 4 Kelompok Transaksi.
* **Model Terbaik:** Decision Tree dengan tuning parameter tertentu.
* **Output:** Model disimpan dalam format `.h5` dan data hasil interpretasi dalam `.csv`.

## 📁 Struktur File
* `proyek-akhir-ml-dicoding-arif.ipynb`: Notebook utama pengerjaan.
* `data_clustering_inverse.csv`: Hasil clustering yang telah di-inverse ke skala asli.
* `model_clustering.h5` & `PCA_model_clustering.h5`: Model Unsupervised.
* `tuning_classification.h5`: Model Supervised hasil tuning.

## 👤 Author
**Arif Purnomo Aji**
dibuat untuk Dicoding Submission: Membangun Proyek Machine Learning 