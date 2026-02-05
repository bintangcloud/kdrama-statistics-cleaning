# 📊 Statistik Dasar & Data Cleaning: K-Drama Dataset

> **Project Status:** *Completed (Mini Task 2)* ✅

Repository ini berisi dokumentasi proses **Data Cleaning** dan perhitungan **Statistik Dasar** pada dataset Drama Korea. Tujuan proyek ini adalah mempersiapkan data yang bersih dan mendapatkan *insight* awal melalui analisis deskriptif.

## 🎯 Tujuan (Objectives)
1.  **Data Cleaning:** Memastikan data bebas dari error (encoding), duplikat, atau format yang tidak konsisten.
2.  **Statistik Dasar:** Mengukur *Central Tendency* (Mean, Median) dan distribusi data (Skewness) untuk variabel Rating dan Episode.

## 📂 Dataset Info
- **Sumber:** [Kaggle](https://www.kaggle.com/datasets/saikalbatyrbekova/korean-dramas-dataset-eda)
- **Data:** 350 Judul Drama
- **Variabel Utama:** `Rating`, `Number of Episodes`, `Year of Release`.

---

## 🛠️ Proses & Hasil (Mini Task 2)

Proses ini dilakukan menggunakan **Microsoft Excel**. Berikut adalah rangkuman langkah-langkah yang dilakukan:

### 1. Data Cleaning Log
Berdasarkan hasil *assessment*, kualitas data sudah cukup baik. Hanya ditemukan masalah minor pada teks deskripsi.

| Masalah Ditemukan (Issue) | Teknik Cleaning | Tindakan (Action) |
| :--- | :--- | :--- |
| **Encoding Error** | Standardization | Memperbaiki karakter simbol aneh (seperti `â€™`) pada kolom *Description* menjadi format teks standar. |
| **Data Verification** | Audit & Imputation | Memverifikasi adanya *Missing Value* (Data Kosong) pada 5 kolom *Genre*,*Tags*, dan *Actors* yang kemudian di isi dengan *Unknown*. Serta tidak ditemukan *Duplicate* (Data Ganda) pada kolom utama. |
| **Invalid Format** | Type Conversion | Memvalidasi bahwa kolom **Rating** dan **Episodes** sudah berformat *Numeric* (bukan Text) agar perhitungan statistik akurat. |

### 2. Statistik Dasar (Insights)
Hasil perhitungan statistik deskriptif menunjukkan:

* **Rating (Mean: 8.65):**
    * Distribusi data **Left Skewed (-0.68)**.
    * *Insight:* Mayoritas Drama Korea memiliki rating tinggi (di atas rata-rata), menunjukkan kepuasan penonton yang tinggi.
* **Episode (Modus: 16):**
    * Distribusi data **Right Skewed (4.92)**.
    * *Insight:* Sebagian besar drama mengikuti format standar 16 episode. Drama dengan episode sangat panjang (>50) adalah *outlier* (biasanya drama keluarga/harian).
* **Korelasi (0.27):**
    * Hubungan antara jumlah episode dan rating sangat lemah. Durasi panjang tidak menjamin rating tinggi.

---

## 👤 Author
**Ni Putu Bintang Permatasari**
*Computer Science Student*
