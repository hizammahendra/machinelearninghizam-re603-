# Supervised Learning - Regresi (USA Housing)

## Deskripsi Proyek

Proyek ini bertujuan untuk membangun model machine learning berbasis regresi guna memprediksi harga rumah menggunakan dataset USA Housing. Pendekatan yang digunakan adalah supervised learning dengan algoritma regresi linear.

Dataset berisi beberapa fitur numerik seperti pendapatan rata-rata area, usia rumah, jumlah kamar, jumlah kamar tidur, dan populasi area, yang digunakan untuk memprediksi harga rumah.

## Dataset

Dataset yang digunakan adalah USA Housing Dataset.

Fitur dalam dataset:

* Avg. Area Income: rata-rata pendapatan di area
* Avg. Area House Age: rata-rata usia rumah
* Avg. Area Number of Rooms: rata-rata jumlah kamar
* Avg. Area Number of Bedrooms: rata-rata jumlah kamar tidur
* Area Population: populasi area
* Price: target yang diprediksi

## Tahapan Proyek

1. Data Loading
   Dataset dibaca menggunakan pandas dan diperiksa strukturnya.

2. Exploratory Data Analysis (EDA)
   Analisis distribusi data dan hubungan antar fitur dilakukan untuk memahami pola.

3. Data Preprocessing
   Tidak dilakukan encoding karena semua fitur numerik. Data langsung dipisahkan menjadi fitur (X) dan target (y).

4. Splitting Data
   Dataset dibagi menjadi data training dan testing.

5. Model Training
   Model regresi linear dilatih menggunakan data training.

6. Evaluasi Model
   Evaluasi dilakukan menggunakan:

   * Mean Absolute Error (MAE)
   * Mean Squared Error (MSE)
   * Root Mean Squared Error (RMSE)

## Model yang Digunakan

Model utama yang digunakan adalah Linear Regression.

Model ini dipilih karena:

* sederhana dan mudah diinterpretasikan
* cocok untuk hubungan linear antar variabel
* baseline yang baik untuk masalah regresi

## Hasil

Model mampu melakukan prediksi harga rumah dengan cukup baik berdasarkan fitur yang tersedia. Nilai error menunjukkan bahwa model sudah dapat menangkap pola utama dalam data, meskipun masih terdapat ruang untuk peningkatan performa.

## Perbaikan yang Dilakukan

Beberapa perbaikan dilakukan pada notebook:

* memperbaiki pemilihan target variabel
* menghindari penghapusan fitur penting
* memastikan visualisasi tidak menyebabkan error
* merapikan alur kode agar lebih konsisten


## Kesimpulan

Pendekatan regresi linear cukup efektif untuk memprediksi harga rumah pada dataset ini. Namun, untuk meningkatkan akurasi, dapat dicoba model lain seperti decision tree atau ensemble methods.

