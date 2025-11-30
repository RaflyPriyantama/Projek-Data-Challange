# Projek-Data-Challange

## Analisis Sentimen Pengguna Shopee COD 2025 Menggunakan Regresi Logistik (GLMNET)

Repositori ini berisi kode, fungsi, dan hasil analisis untuk memodelkan sentimen pengguna Shopee terhadap fitur Cash on Delivery (COD) tahun 2025. Analisis dilakukan menggunakan regresi logistik dengan package **glmnet** di R.

### 📌 Tujuan Proyek
1. Melakukan analisis sentimen berbasis data ulasan Shopee COD.
2. Membangun model klasifikasi biner (positive vs negative).
3. Melakukan pemilihan fitur menggunakan *information gain*.
4. Mengevaluasi performa model menggunakan Confusion Matrix dan AUC (Area Under Curve).

### ⚙️ Fungsi Utama: `glmnet_sentiment()`
Fungsi ini:
- Melakukan filtering data (positive/negative)
- Melakukan train-test split
- Seleksi fitur berbasis *information gain*
- Melatih model regresi logistik penalized (glmnet)
- Menghasilkan:
  - AUC
  - Confusion Matrix
  - Prediksi
  - Daftar fitur terpilih

### 📈 Hasil Utama
Model menghasilkan performa sebagai berikut (berdasarkan hasil eksperimen):

- **AUC:** sekitar 0.86  
- **Akurasi:** ±82%  
- **Kappa:** ±0.60  
- Model mampu membedakan sentimen positif dan negatif dengan cukup baik.

### 🛠️ Library yang Digunakan
- `readr`
- `dplyr`
- `caret`
- `glmnet`
- `pROC`
- `FSelectorRcpp`
