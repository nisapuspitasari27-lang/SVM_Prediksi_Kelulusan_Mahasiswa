# SVM_Prediksi_Kelulusan Mahasiswa
Proyek Klasifikasi SVM untuk Prediksi Kelulusan Mahasiswa.

#  Prediksi Kelulusan Mahasiswa Menggunakan Support Vector Machine (SVM)

## 1. Deskripsi Proyek
Proyek ini bertujuan untuk membangun model klasifikasi *supervised* menggunakan algoritma **Support Vector Machine (SVM)** untuk memprediksi Status Kelulusan Mahasiswa ('TEPAT' atau 'TERLAMBAT') berdasarkan data riwayat akademik dan demografi.

## 2. Dataset
- **File:** `datakelulusanmahasiswa.xlsx - Sheet1.csv`
- **Fitur Kunci:** IPK, IPS 1-8, UMUR, JENIS KELAMIN, STATUS MAHASISWA, STATUS NIKAH.
- **Label:** STATUS KELULUSAN (TEPAT/TERLAMBAT)

## 3. Langkah Pengerjaan
1.  **Exploratory Data Analysis (EDA):** Analisis statistik deskriptif dan visualisasi distribusi IPK.
2.  **Preprocessing Data:** Penanganan *missing values* (imputasi median), *encoding* kategorikal (One-Hot), pembagian data (80:20), dan **Feature Scaling (StandardScaler)**.
3.  **Training Model:** Melatih SVM dengan kernel Linear dan RBF.
4.  **Hyperparameter Tuning:** Menggunakan `GridSearchCV` untuk mengoptimalkan parameter `C` dan `gamma` pada kedua kernel.
5.  **Evaluasi & Interpretasi:** Perbandingan kinerja model terbaik menggunakan metrik Akurasi, Precision, Recall, dan F1-Score, serta interpretasi fitur berpengaruh.
6.  **Deployment Sederhana:** Implementasi fungsi `predict_status()` untuk prediksi.

## 4. Hasil Evaluasi Model
(Isi bagian ini setelah Anda menjalankan kode dan mendapatkan output final dari `final_comparison`):

| Model | Akurasi Testing | Precision (TEPAT) | F1-Score (TEPAT) |
| :--- | :--- | :--- | :--- |
| **SVM Linear** | `0.9211` | ` 0.93  ` | `  0.90  ` |
| **SVM RBF Dasar** | `0.8947` | ` 0.93    ` | `0.87   ` |
| **Model Terbaik (Tuned)** | `0.9211` | `0.88  ` | ` 0.90   ` |

**Kesimpulan:** Model **[NAMA MODEL TERBAIK]** dengan Akurasi **[AKURASI TERBAIK]%** adalah yang terbaik.

## 5. Cara Menjalankan Notebook
1.  Buka Google Colab atau Jupyter Notebook.
2.  Unggah file `datakelulusanmahasiswa.xlsx - Sheet1.csv` ke lingkungan kerja.
3.  Jalankan file `SVM_kelulusan.ipynb` (notebook ini) secara berurutan.

## 6. Identitas Mahasiswa
- **Nama:** Nisa Puspita Sari
- **NIM:** 2457201002448
