# Study Case KAL (kecerdasan Artifisial Lanjut) - Klasifikasi 

Repositori ini berisi proyek studi kasus klasifikasi yang dikembangkan menggunakan Python. Proyek ini mencakup Eksplorasi Data (EDA), preprocessing, pemodelan Machine Learning, hingga penerapan privasi data (*Differential Privacy*). 

Di dalam repositori ini, terdapat dua studi kasus utama yang dianalisis:
1. **Klasifikasi Diabetes (Pima Indians Diabetes Dataset)** dengan penerapan *Laplace Mechanism*.
2. **Eksplorasi dan Analisis Fitur LBP (Local Binary Pattern)** pada kumpulan data yang bersifat numerik.

## 📂 Struktur Repositori

* **`Klasifikasi_Diabetes_KI7.ipynb`**
  Notebook ini berfokus pada klasifikasi pasien diabetes. Langkah-langkah di dalamnya meliputi:
  * Pengambilan data `diabetes.csv` (Pima Indians Diabetes Dataset).
  * Data preprocessing menggunakan `MinMaxScaler`.
  * Pemodelan klasifikasi menggunakan algoritma **Logistic Regression**.
  * Evaluasi model menggunakan metrik *accuracy* dan *classification report*.
  * **Penerapan Differential Privacy**: Menggunakan library `diffprivlib` untuk menambahkan noise (*Laplace Mechanism*) pada dataset guna melindungi privasi data pasien, lalu membandingkan data sebelum dan sesudah penambahan noise.

* **`Study_Case_KAL_Kelompok_3.ipynb`**
  Notebook ini berfokus pada Exploratory Data Analysis (EDA) tingkat lanjut dari sebuah dataset (`project1_3.csv`) yang memiliki atribut berupa fitur tekstur citra / LBP (`lbp13` hingga `lbp24`) beserta target `Class`. Langkah-langkahnya meliputi:
  * Statistik deskriptif data (mean, min, max, std).
  * Visualisasi distribusi data menggunakan Histogram, Boxplot (untuk mendeteksi outlier), dan KDE plot.
  * Pemeriksaan *skewness* pada seluruh data dan data latih.
  * Penghapusan data duplikat (`drop_duplicates()`).

## 🛠️ Persyaratan dan Instalasi (Prerequisites)

Untuk menjalankan kode di dalam notebook ini, pastikan Anda sudah menginstal Python versi 3.x beserta library berikut:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Cara Menjalankan
Lakukan clone pada repositori ini ke lokal Anda:
```bash
git clone [https://github.com/mauliasugeha/StudyCase-KAL-Klasifikasi.git](https://github.com/mauliasugeha/StudyCase-KAL-Klasifikasi.git)
```

Buka folder proyek tersebut:
```bash
cd StudyCase-KAL-Klasifikasi/StudyCase-KAL-Klasifikasi-main
```

Buka Jupyter Notebook atau unggah file ke Google Colab:
```bash
jupyter notebook
```
Jalankan sel (cells) di dalam notebook secara berurutan. (Catatan: Untuk Study_Case_KAL_Kelompok_3.ipynb, pastikan Anda menyesuaikan path direktori dataset ke lokasi CSV LBP di Google Drive / mesin lokal Anda).

## 👥 Contributors (Kelompok 3)
- Maulia Dwi Anthesa Sugeha
- Latifa Anggia Fitriana
- Irene Noer Ramadhany
- Syifani Adillah Salsabila
