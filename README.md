# fga_fundamental_datascience
Bank customer data analysis includes EDA (Exploratory Data Analysis), mobile banking user classification, and credit score prediction. This project aims to understand customer behavior and build a simple machine learning model in Python.

# 💼 Analisis Data Nasabah: EDA, Klasifikasi, dan Prediksi Skor Kredit

Proyek ini terdiri dari tiga mini-project menggunakan data nasabah:  
1. **📊 Exploratory Data Analysis (EDA)**  
2. **🤖 Klasifikasi Pengguna Mobile Banking**  
3. **📈 Prediksi Skor Kredit (Regresi)**  

Seluruh project dikerjakan dalam Python (Jupyter Notebook in VS Code) dan bertujuan untuk melatih kemampuan analisis data, klasifikasi, dan regresi berbasis machine learning sederhana.

---

## 📊 Project 1: Exploratory Data Analysis (EDA) Nasabah

### 🎯 Tujuan
Memahami perilaku dan karakteristik nasabah dari data numerik dan kategorikal.

### 🔍 Analisis Utama:
- **Distribusi variabel numerik**: umur, pendapatan, saldo rata-rata, skor kredit
- **Perbandingan jenis kelamin** terhadap: pendapatan, saldo, skor kredit
- **Frekuensi kunjungan cabang vs pengguna mobile banking**
- **Visualisasi korelasi antar fitur numerik**
- **Produk favorit nasabah** berdasarkan kolom `jenis_produk`
- **Insight singkat** dari tiap variabel dan visualisasi

### 🛠️ Tools & Visualisasi:
- Histogram, Boxplot, Bar chart
- Heatmap korelasi
- Pie chart / Countplot produk

---

## 🤖 Project 2: Klasifikasi Pengguna Mobile Banking

### 🎯 Tujuan
Memprediksi siapa yang cenderung menggunakan mobile banking dari perilaku dan profil keuangan nasabah.

### 🏷️ Target (Y)
`pengguna_mobile_banking` (0 = tidak, 1 = ya)

### 🔡 Fitur (X)
- umur  
- pendapatan  
- saldo_rata_rata  
- jumlah_transaksi  
- frekuensi_kunjungi_cabang  
- jenis_kelamin (encoded)  
- jenis_produk (encoded)  

### 📋 Langkah Analisis:
1. **Preprocessing**:
   - Cek missing value
   - Label encoding untuk fitur kategorikal
2. **Train-test split** (misal 80:20)
3. **Modeling**:
   - Logistic Regression
   - Bonus: Decision Tree Classifier
4. **Evaluasi Model**:
   - Accuracy
   - Precision & Recall
   - Confusion Matrix
5. **Visualisasi**:
   - Heatmap confusion matrix
   - Visualisasi decision tree

### 💡 Insight:
- Faktor penting yang memengaruhi penggunaan mobile banking
- Efektivitas model prediksi

---

## 📈 Project 3: Prediksi Skor Kredit (Regresi)

### 🎯 Tujuan
Memprediksi skor kredit berdasarkan karakteristik dan perilaku finansial nasabah.

### 🏷️ Target (Y)
`skor_kredit`

### 🔡 Fitur (X)
Semua kolom kecuali `nasabah_id` dan `skor_kredit`

### 📋 Langkah Analisis:
1. **Preprocessing**:
   - Cek dan tangani missing value
   - Encoding variabel kategorikal
   - Normalisasi jika diperlukan
2. **Train-test split**
3. **Modeling**:
   - Linear Regression
   - Bonus: Random Forest Regressor
4. **Evaluasi Model**:
   - MAE (Mean Absolute Error)
   - RMSE (Root Mean Squared Error)
   - R² Score (opsional)
5. **Visualisasi**:
   - Scatter plot antara skor aktual dan prediksi
   - Feature importance dari Random Forest

### 💡 Insight:
- Seberapa baik model memprediksi skor kredit
- Fitur paling berpengaruh dalam menentukan skor kredit

---

## 🛠️ Tools & Library yang Digunakan
- Python (Jupyter Notebook)
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 📁 Output
Setiap project disusun dalam format notebook `.ipynb` yang berisi:
- Visualisasi data
- Kode analisis
- Markdown insight per tahap
