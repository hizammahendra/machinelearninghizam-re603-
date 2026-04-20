# Data Exploration and Data Visualization

Proyek ini berisi proses Exploratory Data Analysis (EDA) dan Feature Engineering menggunakan dataset:

* california_dataset.csv
* company.csv

## Tujuan

Melakukan analisis awal data serta preprocessing untuk mempersiapkan data sebelum digunakan dalam model Machine Learning.

## Tahapan Pengerjaan

### 1. Analisis Distribusi dan Outlier

Visualisasi dilakukan menggunakan:

* Histogram
* Q-Q Plot
* Boxplot

Kolom yang dianalisis:

* MedInc
* HouseAge
* AveRooms
* AveBedrms
* AveOccup

### 2. Handling Outlier

Metode yang digunakan adalah Interquartile Range (IQR) dengan teknik capping.
Contoh penerapan dilakukan pada kolom HouseAge.

### 3. Missing Value Handling

Dilakukan pada kolom Headquarters dengan langkah:

* Mengecek persentase missing value
* Drop kolom jika lebih dari 20%
* Jika tidak, dilakukan imputasi (median atau modus sesuai tipe data)

## Tools

* Python
* Pandas
* Matplotlib
* Scipy

