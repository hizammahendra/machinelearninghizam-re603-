# Klasifikasi Pemain NBA Menggunakan KNN

## Deskripsi
Proyek ini bertujuan untuk melakukan klasifikasi pemain NBA berdasarkan status **active_player** menggunakan algoritma K-Nearest Neighbors (KNN). Dataset yang digunakan berisi statistik pemain seperti total poin, jumlah pertandingan, dan rata-rata poin per game.

---

## Dataset
Dataset memiliki beberapa fitur utama:

- rank  
- position  
- total_points  
- total_games  
- points_per_game  
- field_goals  
- three_points_goals  
- free_shots  
- born  
- active_player (target)  

---

## Alur Proyek

### 1. Exploratory Data Analysis (EDA)
Dilakukan untuk memahami struktur data, distribusi, serta mendeteksi nilai yang tidak konsisten, khususnya pada kolom `born`.

### 2. Preprocessing
- Mengubah kolom `born` menjadi numerik  
- Menghapus kolom yang tidak relevan  
- Melakukan encoding pada data kategorikal  
- Menangani missing values  

### 3. Modelling
Model yang digunakan adalah K-Nearest Neighbors dari scikit-learn:

```python
from sklearn.neighbors import KNeighborsClassifier
```

### Hasil Evaluasi

Accuracy: 0.93
Precision: 0.47
Recall: 0.50
F1-Score: 0.48

Confusion Matrix:

[[14  0]
 [ 1  0]]

### Analisis

Meskipun nilai akurasi tinggi, model tidak mampu memprediksi kelas minoritas (active_player = 1). Hal ini disebabkan oleh ketidakseimbangan data, sehingga model cenderung memprediksi kelas mayoritas.


### Kesimpulan

Model KNN dapat digunakan untuk klasifikasi data pemain NBA, namun performanya dipengaruhi oleh distribusi data. Ketidakseimbangan data menyebabkan model kurang efektif dalam mendeteksi kelas minoritas.
 
